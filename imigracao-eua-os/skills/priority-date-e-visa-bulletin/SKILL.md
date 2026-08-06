---
name: priority-date-e-visa-bulletin
description: "Priority date, Visa Bulletin (Final Action × Dates for Filing), retrogressão e concurrent filing. ⛔ Nenhuma data de corte no texto — mudam todo mês. Use em filas F1–F4, EB, DV rank, quando perguntar 'quando sai o green card', I-485 timing e charts do USCIS."
---

# PRIORITY DATE · VISA BULLETIN · RETROGRESSÃO

> **Camada C4 · Green card.** Frentes: 👤 imigrante · ⚖️ advogado.  
> (💼 usa o mapa para expectativa honesta de prazo — sem prometer data.)  
> Hub: https://www.uscis.gov/green-card/green-card-processes-and-procedures/visa-availability-priority-dates  
> Retrogressão: https://www.uscis.gov/green-card/green-card-processes-and-procedures/visa-availability-priority-dates/visa-retrogression  
> Charts AOS (qual chart o USCIS usa no mês): https://www.uscis.gov/green-card/green-card-processes-and-procedures/visa-availability-priority-dates/adjustment-of-status-filing-charts-from-the-visa-bulletin  
> **Visa Bulletin (DOS) — sempre o do mês corrente:**  
> https://travel.state.gov/content/travel/en/legal/visa-law0/visa-bulletin.html  
> Gate: `varredura-de-vigencia` (camada 3).

---

## 1. ⛔ TRAVA — zero cut-off no texto

| Proibido | Correto |
|---|---|
| “O cut-off do Brasil em F4 é [data]” | Abrir o **Visa Bulletin do mês** + chart USCIS; citar **data da consulta** |
| Tabela de datas na skill / proposta / e-mail “congelada” | Link + “leia o mês vigente” |
| Prometer “sai em X meses” pela fila | Fila **move e retrocede**; só mecanismo + URL |

Cut-offs mudam **todo mês, por desenho**. Esta skill ensina o **mecanismo**, não o número do mês.

---

## 2. O que é *priority date*

A **priority date** é a data que posiciona o alien na fila da preferência (family ou employment). Em geral:

| Situação | Priority date = |
|---|---|
| Family preference | Data em que o **I-130** (ou, em certos casos, **I-360**) foi *properly filed* |
| Employment **com** labor certification | Data em que o **DOL aceita** a labor cert para processamento; o I-140 deve ser protocolado **dentro da validade** da cert (ver página I-140) |
| Employment **sem** labor cert | Data em que o USCIS **aceita** o **I-140** |
| EB-4 / special immigrant (incl. religioso) | Data em que o USCIS aceita o **I-360** |
| EB-5 | Data em que o USCIS aceita o **I-526** / **I-526E** (checar retenção RIA na página do dia se o caso for retention) |

Fonte da tabela: hub de *visa availability / priority dates* (URL acima).  
*Immediate relatives* **não** usam fila de preferência da mesma forma — vistos tratados como sempre disponíveis (skill `familia-ir-e-preferencias`).

---

## 3. Os **dois** charts do Visa Bulletin

O DOS publica mensalmente (mecanismo USCIS/DOS):

### A) *Application Final Action Dates*

Quando um visto imigrante pode ser **emitido** / quando o AOS pode ser **aprovado** (ação final).

### B) *Dates for Filing Applications*

Quando se pode **montar** o caso / quando o USCIS **pode** aceitar o **I-485** (se o USCIS autorizar o uso desse chart no mês).

### Qual chart o USCIS usa para I-485?

Regra USCIS (texto do hub):

> Salvo indicação em contrário na página **Adjustment of Status Filing Charts from the Visa Bulletin**, use **Application Final Action Dates** para decidir se pode protocolar o I-485.

Quando o DOS/DHS entendem que há mais vistos do que *applicants* conhecidos, o USCIS pode autorizar o chart **Dates for Filing**.  
**Sempre** cruzar:

1. Bulletin do mês em `travel.state.gov`  
2. Página de **filing charts** do USCIS (URL acima)

Códigos típicos: **“C”** = *current* (disponível de imediato); **“U”** = *unavailable*.  
Visto “disponível” na leitura de cut-off: priority date **anterior** à data de corte da categoria/país de *chargeability* (regra da página priority dates — sem colar datas).

---

## 4. Retrogressão (*visa retrogression*)

Hub: URL de retrogression acima.

- Ocorre quando **mais pessoas** pedem visto em uma categoria/país do que há **vistos no mês**.  
- Uma priority date que “passava” num mês pode **deixar de passar** no seguinte.  
- No início do **ano fiscal** (1º de outubro) há novo suprimento de vistos — as datas **costumam** (mas **nem sempre**) melhorar.

### Efeito no I-485 já protocolado

- Caso pode ficar **em abeyance** até o visto voltar a estar disponível.  
- Benefícios incidentais (ex.: EAD I-765, Advance Parole I-131) **podem** continuar disponíveis se o I-485 foi *properly filed* antes da retrogressão — confirmar nas páginas dos forms no dia.  
- ⛔ Retrogressão **não** é “negativa do green card”; é **falta de número** no mês.

---

## 5. Concurrent filing (ligação prática)

https://www.uscis.gov/green-card/green-card-processes-and-procedures/concurrent-filing-of-form-i-485

- Concurrent = I-485 **antes** da aprovação da petição subjacente (junto ou enquanto pendente).  
- **IR:** concurrent em geral permitido.  
- **Preferências / EB:** só se o visto estiver **imediatamente disponível** (charts do mês).  
- **Não** existe concurrent filing no processamento **consular** puro.

---

## 6. Protocolo de saída (obrigatório)

```text
## Visa Bulletin / priority date
- Data da consulta: AAAA-MM-DD
- Priority date do caso: AAAA-MM-DD (fonte: form/receipt)
- Categoria + chargeability:
- Bulletin lido: <URL do mês>
- Chart usado para a pergunta (Final Action / Filing) + se USCIS liberou Filing:
- Resultado: CURRENT | NÃO CURRENT | UNAVAILABLE | FALHA DE LEITURA
- ⛔ Se travel.state.gov bloquear: declarar falha — não inventar cut-off
```

Isso é a materialização da **camada 3** de `varredura-de-vigencia`.

---

## 7. O que cada frente faz

| 👤 | ⚖️ | 💼 |
|---|---|---|
| Entende: fila ≠ “processando”; cut-off muda; retrogressão existe | Aplica charts corretos ao I-485; CSPA/*aging out* quando o filho envelhece na fila | Expectativa honesta; **nunca** data prometida de aprovação |

## Encadeamento

Skills de categoria (família/EB/DV) → **esta** → `ajuste-x-consular` → protocolar só com dossiê completo (TRAVA 2).

## Guard

1. **Dois charts** — Final Action × Dates for Filing; USCIS default = Final Action salvo chart page.  
2. **Retrogressão** explicada sem drama falso nem promessa.  
3. ⛔ **Nenhuma** data de corte no corpo da skill.  
4. Priority date: tabela de fixação + URL.  
5. Falha de leitura do DOS = gap declarado, não invenção.
