---
name: linha-do-tempo-do-caso
description: "Monta a linha do tempo do caso de imigração EUA: marcos, filas e o que trava cada etapa. Sem processing time hardcoded — só dependências e URLs oficiais no dia. Use após escolher a rota (mapa-de-caminhos), quando houver petição pendente, priority date, RFE, ou o cliente perguntar 'em que pé está / o que vem depois'."
---

# LINHA-DO-TEMPO-DO-CASO — marcos, filas e travas

> **Camada C2 · Triagem e diagnóstico.** Frentes: 👤 imigrante · ⚖️ advogado.  
> 💼 usa a linha para explicar o serviço e **não** prometer data de aprovação.  
> Anexos: `context/anexo-ina-estatuto.md` · `context/anexo-nao-imigrante.md`.  
> Gates: `varredura-de-vigencia` (Visa Bulletin, taxas, TPS, H.R.1); `trava-de-representacao` se a etapa for aparência inland.

## Princípios

1. **Marco ≠ prazo de governo.** A skill lista **o que precisa acontecer** e **o que bloqueia** — não “sai em N dias”.
2. **Números de fila/taxa/processing** → URL + data de consulta. Nunca cache de treino (TRAVA 3).
3. **Fase errada** é o erro operacional: tratar *priority date* futura como “já pode imigrar”; tratar RFE como opcional; tratar I-94 expirado como detalhe.
4. Desde **PA-2026-05**, protocolo incompleto pode **morrer no primeiro marco** (negativa sem RFE/NOID).  
   PDF: https://www.uscis.gov/sites/default/files/document/policy-manual-updates/20260805-EvidentiaryStandards.pdf

---

## 1. Identificar o **tipo de linha** (botões / classificação)

| Tipo | Trilha típica | âncora estatutária / reg |
|---|---|---|
| **A. Não-imigrante consular** | B, F, J, H… via visto + CBP | `8 U.S.C. 1184` · `8 CFR 214` · 22 CFR visto |
| **B. Não-imigrante mudança/extensão** | I-129 / I-539 nos EUA | `8 CFR 214` · `8 CFR 248` |
| **C. Imigrante familiar/emprego** | I-130 / I-140 → fila → visto ou AOS | `8 U.S.C. 1151`–`1153` · `1154` · `1255` |
| **D. Humanitário** | I-589, TPS, U/T/VAWA… | regras próprias; vigência no dia |
| **E. Contencioso** | RFE/NOID, I-290B, NTA, EOIR | `8 CFR 103` · EOIR; só com rep autorizada |

eCFR part 214: https://www.ecfr.gov/current/title-8/chapter-I/part-214  
eCFR part 248: https://www.ecfr.gov/current/title-8/chapter-I/part-248  
uscode título 8: https://uscode.house.gov/

---

## 2. Marcos canônicos (preencher só os do tipo)

### Tipo A — NI consular

| # | Marco | O que trava |
|---|---|---|
| A1 | Elegibilidade + dossiê (laços, propósito) | 214(b) se intenção/permanentismo; dossiê fraco |
| A2 | DS-160 / taxa consular (URL no dia) | Dados inconsistentes; *misrepresentation* |
| A3 | Entrevista no posto | 214(b), 221(g), documentos faltantes |
| A4 | Visto emitido / recusado / 221(g) | Condicionantes do consular |
| A5 | Admissão CBP (I-94 / status) | Grounds of inadmissibility na fronteira |
| A6 | Manutenção de status | *Overstay* → calcular UP e eventual barra 212(a)(9)(B). Trabalho não autorizado = *failure to maintain status* (`8 CFR 214.1(e)`); UP/barras exigem análise separada |

### Tipo B — EOS / COS nos EUA

| # | Marco | O que trava |
|---|---|---|
| B1 | Status **atual** válido na data do pedido | Já fora de status → outra linha + `barras-3-10-anos` |
| B2 | Form correto (I-129 vs I-539) + *initial evidence* | Negativa sem RFE (PA-2026-05) |
| B3 | Biometrics / RFE se emitido | Prazo do **notice** (teto, não “padrão”); correio internacional **+3** dias sob `8 CFR 103.8(b)` — **não** +14 |
| B4 | Aprovação e novo prazo de admissão | Violação entre pedido e decisão |
| B5 | Dependentes | Status derivado amarrado ao principal |

`8 CFR 103.8`: https://www.ecfr.gov/current/title-8/chapter-I/part-103/section-103.8  
Resposta a RFE: skill `resposta-a-rfe-noid`.

### Tipo C — Green card (família / emprego)

| # | Marco | O que trava |
|---|---|---|
| C1 | Petição base (I-130 / I-140 / EB-5 etc.) | Prova de vínculo, labor, investimento; dossiê incompleto |
| C2 | Aprovação da petição | RFE/NOID/negativa; revogação |
| C3 | *Priority date* corrente? | **Visa Bulletin do mês** — https://travel.state.gov — ler no dia |
| C4 | Escolha **AOS (I-485)** vs **consular (NVC/DS-260)** | Elegibilidade 245; presença; risco de saída com UP — `ajuste-x-consular` |
| C5 | *Affidavit of support* / exames / civil docs | I-864 incompleto; ponte BR (certidão, apostila) |
| C6 | Entrevista / decisão LPR | Inadmissibilidade 212(a); fraude |
| C7 | Condicional (se houver) → remoção de condições | Casamento/investimento não sustentado |

Cotas/preferências: `8 U.S.C. 1153` — https://uscode.house.gov/view.xhtml?req=granuleid:USC-prelim-title8-section1153  
Ajuste: `8 U.S.C. 1255` — https://uscode.house.gov/view.xhtml?req=granuleid:USC-prelim-title8-section1255

### Tipo D — Humanitário (esqueleto)

| # | Marco | O que trava |
|---|---|---|
| D1 | Qualificação fática + formulário | Prazo de asilo, coabitação VAWA, etc. (skill da categoria) |
| D2 | Vigência do programa (TPS/parole…) | *Designado* ≠ *vigente* — country page **no dia** |
| D3 | Fees anuais / notices (ex.: AAF em asilo) | Não pagar no prazo do notice → rejeição / perda de benefício — **sem** inventar valor |
| D4 | Entrevista / decisão / EAD | Regras próprias; não generalizar RFE do PA-2026-05 ao asilo sem ler a exceção |

### Tipo E — Contencioso

| # | Marco | O que trava |
|---|---|---|
| E1 | Ler o notice (RFE/NOID/NTA/decisão) | Prazo no **documento**, não na memória |
| E2 | Quem representa | 292.1 — inland: só hipóteses fechadas de 292.1(a)(1)-(5) (cada qual sob seus requisitos); só-OAB não é *attorney* de 8 CFR 1.2. Fora: (a)(6)+G-28I discricionário. EOIR: chapter V separado |
| E3 | Resposta / motion / recurso | Tese + prova; prazo teto |
| E4 | EOIR / BIA / AAO | Só com representação autorizada — `removal-eoir-bia-aao` |

---

## 3. Formato de saída

```text
## Linha do tempo do caso
- Data da montagem: AAAA-MM-DD
- Tipo: A|B|C|D|E (+ categoria)
- Situação atual: [marco em que o caso ESTÁ]
- Fora de status / UP? [sim→barras-3-10-anos]

### Marcos
| Ordem | Marco | Status (feito/pendente/bloqueado) | O que trava | Fonte/URL se móvel |
|---|---|---|---|---|
| 1 | … | … | … | … |

### Fila / vigência (se aplicável)
- Visa Bulletin: consultado? URL + data | N/A
- TPS/programa: country page + data | N/A
- Taxas do próximo protocolo: G-1055 + data | N/A

### Próximo ato humano
- [ ] o que o cliente faz
- [ ] o que o dossiê BR faz
- [ ] o que o attorney EUA faz (se inland)
- Sem promessa de data de decisão do governo.
```

Processing times (se o usuário insistir em “quanto demora”): mandar https://egov.uscis.gov/processing-times/ **com data de consulta** e dizer que **não** é garantia — *Avoid Scams*: https://www.uscis.gov/avoid-scams

---

## Travas transversais em qualquer linha

| Trava | Efeito na linha do tempo |
|---|---|
| **TRAVA 2** PA-2026-05 | Marco “protocolar” exige dossiê completo — skill `dossie-pre-protocolo` |
| **TRAVA 3** | Nenhum cut-off/fee/processing no corpo |
| **UP / barras** | Saída após UP pode **inserir** anos de bloqueio — `barras-3-10-anos` |
| **Linha geográfica** | Marcos de “audiência / field office / EOIR” exigem rep autorizada |
| **PM ≠ lei** | Marco legal vem do estatuto/CFR; PM guia o oficial |

`8 CFR 292.1`: https://www.ecfr.gov/current/title-8/chapter-I/part-292/section-292.1

## O que esta skill **não** faz

- Não calcula dias de processamento nem de *unlawful presence*.
- Não redefine elegibilidade (isso é o diagnóstico).
- Não redige resposta a RFE (só posiciona o marco).
- Não promete data de entrevista ou de green card.

## Encadeamento

`mapa-de-caminhos` (rota escolhida) → **esta** → skill de categoria / `dossie-pre-protocolo` / `resposta-a-rfe-noid` / `priority-date-e-visa-bulletin`.

## Guard

1. Marcos + **o que trava** cada um — sem número de prazo de governo.  
2. Fila e cut-off só com Visa Bulletin / fonte do dia.  
3. RFE: prazo do notice; correio internacional +3 (`103.8(b)`), não +14.  
4. Fora de status → não montar linha “otimista” sem `barras-3-10-anos`.  
5. Zero taxa/cota hardcoded.  
6. Citar gates C1; não reescrevê-los.
