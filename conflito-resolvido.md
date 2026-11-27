# Registro do conflito resolvido

## O que aconteceu

Para praticar a resolução de conflitos, editei a mesma linha do README (a primeira frase de apresentação do guia) em dois lugares diferentes:

- Na branch `review/linguagem`, reescrevi a frase para deixar a linguagem mais simples.
- Na `main`, mudei a mesma frase de outro jeito, deixando mais claro quem é o público do guia.

Quando rodei `git merge review/linguagem` na `main`, o Git não conseguiu decidir sozinho qual versão manter e marcou o conflito no arquivo.

## Como o conflito apareceu

```
<<<<<<< HEAD
Este guia é uma introdução à inflação para estudantes de Economia e para quem quer entender por que os preços sobem.
=======
Este guia apresenta, de forma simples, o que é inflação e como ela afeta o dia a dia.
>>>>>>> review/linguagem
```

A parte entre `<<<<<<< HEAD` e `=======` é a versão da `main`. A parte entre `=======` e `>>>>>>> review/linguagem` é a versão da branch.

Um detalhe que eu não esperava: na branch review/linguagem eu também tinha trocado "eu incluído" por "inclusive eu" no segundo parágrafo do README. Essa mudança não gerou conflito, e o Git juntou sozinho, porque só a branch tinha mexido naquela linha. O conflito ficou só na frase que as duas branches alteraram.


## Decisão

As duas versões tinham uma parte boa: a da `main` deixava claro o público, e a da branch explicava melhor do que o guia trata. Em vez de escolher uma, juntei as duas ideias:

```
Este guia apresenta, de forma simples, o que é inflação e como ela afeta o dia a dia, pensado para estudantes de Economia e para quem quer entender por que os preços sobem.
```

## Resolução

1. Abri o README e apaguei os marcadores `<<<<<<<`, `=======` e `>>>>>>>`.
2. Deixei só a frase final, combinando as duas versões.
3. Rodei `git add README.md` para marcar o conflito como resolvido.
4. Rodei `git commit` para concluir o merge.

O commit de merge aparece no histórico do repositório (`git log --oneline --graph --decorate --all`).
