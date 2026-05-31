# Modelo de domínio — conciliação de adquirência (sintético)

> **Tarefa da Semana 1 (sua, Wellington).** Este é o exercício de *design do zero*.
> Preencha as 3 seções abaixo com SUAS decisões. Não precisa de código ainda — só o desenho.
> O mentor revisa, questiona os trade-offs e fechamos o diagrama juntos.
>
> ⚠️ Versão **genérica/sintética** — nada da Zig (nomes, regras específicas ou dados reais).

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
