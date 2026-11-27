# Aprendizados

Antes deste projeto, eu usava o Git praticamente só para guardar arquivos no GitHub, sempre na mesma branch e com commits grandes. Fazer o guia com um fluxo mais organizado mudou a forma como eu vejo a ferramenta.

## Branches

Separar o trabalho em branches (uma para o README, outra para o conteúdo, outra para os exercícios e uma para revisar a linguagem) deixou mais fácil saber o que eu estava fazendo em cada momento. Se alguma parte desse errado, a `main` continuaria funcionando.

## Commits atômicos

Fazer um commit para cada mudança, com mensagens no padrão docs: e merge:, deu um pouco mais de trabalho no começo, mas o histórico ficou fácil de ler. Olhando o `git log`, dá para entender a ordem em que o guia foi construído sem abrir nenhum arquivo.

## Pull request

Abrir o pull request me fez revisar o conteúdo antes de juntar na `main`. O checklist ajudou a lembrar de coisas que eu teria esquecido, como testar os links entre as páginas.

## Conflito

O conflito foi a parte que eu mais tinha receio, mas depois de ver os marcadores no arquivo ficou claro que ele só mostra as duas versões e espera eu decidir. A decisão está registrada em [conflito-resolvido.md](conflito-resolvido.md).

## O que eu levaria para outros projetos

Usaria esse mesmo fluxo nos meus códigos em R da faculdade, principalmente o hábito de trabalhar em branches e escrever mensagens de commit claras. Também usaria o `.gitignore` desde o início para não subir arquivos de dados grandes ou gerados automaticamente.
