# payments-analytics-starter

> Projeto de referência de **Analytics Engineering para adquirência / meios de pagamento**:
> dados sintéticos de transações e liquidação, modelagem em dbt e uma camada de **conciliação**
> (esperado × liquidado) com métricas de negócio. **Sem nenhum dado real** — tudo sintético.

🚧 **Status:** em construção (Semana 1 — modelagem do domínio).

## Por que este projeto existe
Demonstrar, de forma pública e verificável, a modelagem de um **data product de pagamentos
do zero**: do dado bruto às métricas que o negócio consome (taxa de conciliação, MDR, taxa de
aprovação), incluindo a lógica de **classificação de status de conciliação** (conciliado /
não conciliado por adquirente / não conciliado interno).

## Arquitetura pretendida
```
data_generator/   → gera dados sintéticos: transações + liquidação (EDI) das adquirentes
dbt_project/      → staging → intermediate → marts (conciliação + métricas)
docs/             → modelo de domínio, decisões e diagramas
```

## Stack
Python · dbt · SQL · (orquestração e camada de IA virão em projetos seguintes)

## Como rodar
_(a documentar conforme o projeto evolui)_

## Roadmap do projeto
- [ ] **Semana 1:** modelo de domínio ([docs/modelo-de-dominio.md](docs/modelo-de-dominio.md))
- [ ] Semana 2: gerador de transações
- [ ] Semana 3: gerador de liquidação + divergências
- [ ] Semana 4: staging (dbt)
- [ ] Semana 5: mart de conciliação + status
- [ ] Semana 6: métricas + testes
- [ ] Semana 7: docs + publicação

---
Autor: [Wellington Vieira](https://github.com/vieira-wj) · Analytics Engineer · Pagamentos & Adquirência
