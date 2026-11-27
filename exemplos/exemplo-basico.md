# Exemplo básico: fazendo as contas da inflação

Este exemplo junta os três cálculos que mais aparecem quando se fala de inflação. Todos usam só porcentagem e potência, e dá para fazer na calculadora do celular.

## 1. Variação de um preço

Um quilo de café custava R$ 40,00 e passou a custar R$ 46,00.

```
variação = (preço novo - preço antigo) / preço antigo
variação = (46 - 40) / 40 = 0,15 → 15%
```

## 2. Inflação acumulada

Suponha uma inflação de 1% ao mês durante 12 meses. Somar os meses daria 12%, mas isso está errado, porque cada aumento é aplicado sobre um preço que já tinha subido.

```
acumulado = (1 + taxa mensal)^número de meses - 1
acumulado = (1,01)^12 - 1 ≈ 0,1268 → 12,68%
```

Quando as taxas mudam de um mês para o outro, a lógica é a mesma: multiplica-se tudo. Com 0,5%, 0,8% e 0,3% em três meses:

```
acumulado = (1,005 × 1,008 × 1,003) - 1 ≈ 0,0161 → 1,61%
```

## 3. Juro real

Uma aplicação rendeu 12% em um ano em que a inflação foi de 5%. O ganho de poder de compra não é 12% - 5% = 7%:

```
juro real = (1 + juro nominal) / (1 + inflação) - 1
juro real = 1,12 / 1,05 - 1 ≈ 0,0667 → 6,67%
```

A subtração simples dá uma boa aproximação quando as taxas são baixas, mas a diferença aumenta quando elas são altas.

---

[Voltar ao início](../README.md)
