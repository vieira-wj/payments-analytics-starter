# Modelo de domínio — conciliação de adquirência (sintético)

> **Exercício de design do zero.** Preencha as 3 seções abaixo com suas decisões, baseadas em
> **como adquirência funciona no mercado em geral (conhecimento público)**. Não precisa de
> código ainda — só o desenho.
>
> ⚠️ **100% genérico e sintético.** Não usar nada específico de sistemas internos de empregadores
> (modelos, regras de negócio, listas ou nomes). Apenas conceitos públicos do setor de pagamentos.

## 1. Entidades
Liste as entidades essenciais para uma conciliação de adquirência e, em uma linha, o que cada
uma representa.

_Exemplo de ponto de partida (edite/adicione/remova à vontade):_
- `transacao` — uma venda capturada (o que o sistema interno registra).
- `liquidacao` (EDI) — o que a adquirente reporta que vai pagar/pagou.
- `adquirente` — ...
- `estabelecimento` — ...
- ...

➡️ **Sua resposta:**
```
(escreva aqui)
```

## 2. Campos da entidade `transacao`
Quais campos mínimos para (a) casar com a liquidação e (b) calcular métricas?
Pense em: identificador (NSU/tid?), valor, taxa, bandeira, método, data, status...

➡️ **Sua resposta:**
| campo | tipo | para que serve |
|---|---|---|
|  |  |  |

## 3. Regra de `status` da conciliação
Quais valores o status pode ter e qual a regra de cada um? (este é o coração do projeto.)

_Sugestão de ponto de partida — ajuste:_
- `conciliado` — transação casou com a liquidação (valor e chave batem).
- `nao_conciliado_adquirente` — ...
- `nao_conciliado_interno` — ...
- `apartada` / outro? — ...

➡️ **Sua resposta:**
```
(escreva aqui — valor: regra)
```

---
## Decisões fechadas (preenchido pelo mentor após revisão)
- _(vazio)_
