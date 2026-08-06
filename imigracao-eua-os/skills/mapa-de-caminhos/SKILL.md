---
name: mapa-de-caminhos
description: "Compara rotas de imigração EUA lado a lado: tempo relativo, custo (só URLs), risco e reversibilidade. Mostra o que dá para desfazer e o que queima a ponte (negativa, misrepresentation, unlawful presence). Use após diagnostico-de-elegibilidade quando há 2+ rotas plausíveis, ou quando o cliente/comercial pede 'qual caminho é melhor'."
---

# MAPA-DE-CAMINHOS — tempo · custo · risco · reversibilidade

> **Camada C2 · Triagem e diagnóstico.** Frentes: 👤 imigrante · 💼 comercial.  
> ⚖️ consome o mapa para estratégia de peça, mas a comparação amigável é 👤/💼.  
> Pré-requisito: `diagnostico-de-elegibilidade` (com **gate zero** de fora de status).  
> Anexos: `context/anexo-ina-estatuto.md` · `context/anexo-nao-imigrante.md`.

## Quando ativar

- Há **duas ou mais** rotas ✅ ou 🟡 no diagnóstico.
- O usuário pergunta “o que é mais rápido / barato / seguro”.
- O comercial precisa escolher **o que vender** sem mentir (captação honesta).

⛔ Se o diagnóstico ainda não perguntou *fora de status* / *unlawful presence* → **voltar** a `diagnostico-de-elegibilidade` + `barras-3-10-anos`.  
⛔ Se a pessoa pede **garantia** de resultado ou prazo → recusar e citar https://www.uscis.gov/avoid-scams

---

## As quatro dimensões (sempre as quatro)

### 1. Tempo (relativo — **sem** processing time hardcoded)

Comparar **ordem de grandeza e dependências**, nunca “X meses”:

| Tipo de marco | Como falar | Onde ler no dia |
|---|---|---|
| Consular (visto NI) | entrevista/agenda depende do posto | https://travel.state.gov · página do posto |
| Petição USCIS | adjudicação + possível RFE/NOID | https://egov.uscis.gov/processing-times/ (URL + data; **não** copiar número na skill) |
| Fila de imigrante | *priority date* × Visa Bulletin | https://travel.state.gov (bulletin do mês) |
| Ajuste vs consular | escolha muda a linha do tempo | skill `ajuste-x-consular` |

Sempre: **varredura-de-vigencia** se citar cut-off ou taxa. Zero cut-off/fee no corpo.

### 2. Custo (só mapa de **componentes** + URL)

Componentes típicos — **valores só no G-1055 / notice / fee do DOS no dia**:

- Taxa de formulário USCIS → https://www.uscis.gov/g-1055  
- Taxas consulares / MRV → https://travel.state.gov  
- Honorário BR (direito brasileiro / dossiê) × honorário *attorney* EUA (se inland)  
- Tradução, apostila, exames, viagem  

⛔ Não escrever dólar de memória. Fees da Pub. L. 119-21 / AAF: se não confirmados no notice, **não inventar**.

### 3. Risco (jurídico e prático)

| Risco | Exemplos |
|---|---|
| **Adjudicatório** | 214(b) em B/F; falta de *initial evidence* → negativa sem RFE (PA-2026-05) |
| **Status** | *overstay*, violação de status, trabalho sem autorização |
| **Inadmissibilidade** | 212(a) — crime, fraude, saúde, presença ilegal |
| **Estratégico** | escolher B como “morar”; misturar intenção; protocolo incompleto |
| **Representação** | prometer G-28 inland só-OAB — `trava-de-representacao` / `8 CFR 292.1` |

PA-2026-05: https://www.uscis.gov/sites/default/files/document/policy-manual-updates/20260805-EvidentiaryStandards.pdf  
214(b): `8 U.S.C. 1184(b)` — https://uscode.house.gov/view.xhtml?req=granuleid:USC-prelim-title8-section1184  
212(a): `8 U.S.C. 1182` — https://uscode.house.gov/view.xhtml?req=granuleid:USC-prelim-title8-section1182

### 4. Reversibilidade ⭐ (obrigatório neste skill)

Toda comparação inclui **o que se desfaz** e **o que queima a ponte**.

#### Em geral **reversível** ou recuperável com custo

| Ação | Por que é (mais) reversível |
|---|---|
| Explorar categorias, montar dossiê, **não** protocolar ainda | Não há adjudicação |
| Retirar / não prosseguir **antes** de fraude | Sem *misrepresentation* no record |
| Trocar de estratégia **antes** de qualquer fraude ou *willful material misrepresentation* em pedido de visto, documento, admissão ou outro benefício | Mudar antes da entrada **não** apaga declaração material falsa já feita sob 212(a)(6)(C) |
| Manter status e laços honestos no exterior (trilha NI) | Preserva opções futuras se a intenção for verdadeira |
| Referral a *attorney* EUA / reestruturar proposta comercial | Compliance; não cria *status* federal falso |
| **Pedido negado** sem achado de fraude | Ler notice/form e mapear *appeal* ou *motion* cabível (`8 CFR 103.3` / `103.5`) — veículo depende do caso; **não** há “res judicata prática” genérica |

#### Em geral **irreversível** ou que queima a ponte

| Ação | Por que queima |
|---|---|
| **Alegação falsa** / *material misrepresentation* em DS-160, petição, entrevista | Inadmissibilidade 212(a)(6)(C); contamina o histórico; avaliar waiver com o subsection aplicável |
| Acumular ***unlawful presence*** e depois **sair** dos EUA | Dispara barras de reentrada — `barras-3-10-anos` |
| Entrar em B-1/B-2 **com plano fixo de imigrar/trabalhar** | 214(b) / fraude de visto — não é “atalho” |
| Protocolar **incompleto** na era PA-2026-05 | Negativa **sem** RFE/NOID — queima tempo, taxa e às vezes a teoria do caso |
| Assinar / vender representação **fora** do 292.1 | UPL + risco ético/criminal; queima o modelo comercial |

Regra de ouro do mapa: **preferir rota com ponte intacta** se a diferença de tempo for só “sensação”. Velocidade vendida com fraude **não** é produto deste plugin.

---

## Tabela de comparação (preencher no caso)

```text
## Mapa de caminhos — [data]
Pré-condição: diagnóstico com gate zero de status = [SIM ok / BLOQUEADO→barras]

| Rota | Tempo (relativo + dependências) | Custo (componentes + URLs) | Risco | Reversibilidade | Veredito |
|---|---|---|---|---|---|
| A … | … | G-1055 / travel.state.gov | … | o que desfaz / o que queima | preferida / alternativa / descartar |
| B … | … | … | … | … | … |

### Recomendação (não garantia)
- Preferida: … porque …
- Descartada: … porque queima / fechada / 🔴
- Próximo: dossie-pre-protocolo | skill de categoria | attorney EUA | barras-3-10-anos
```

### Exemplos de pares (ilustrativos — **não** fecham o caso sem fatos)

| Par | O mapa deve forçar |
|---|---|
| B-2 “rápido” × IR cônjuge | 214(b)/intenção vs fila familiar + dossiê; reversibilidade da mentira no B |
| F-1 × H-1B × EB-2 | estudo com laços vs dual-intent vs green card; regime F em transição (skill `estudante-f-m`) |
| Ajuste inland × consular | presença nos EUA, elegibilidade 245, risco de saída com UP |
| “Protocolar agora incompleto” × dossiê completo | TRAVA 2 — incompleto **não** é atalho desde PA-2026-05 |

---

## Por frente

| Frente | Uso do mapa |
|---|---|
| 👤 | Entender trade-offs sem jargão; ver o que **não** dá para desfazer |
| 💼 | Escolher o que **entrar na proposta**; se a rota queima ponte, **não vender** (`captacao-honesta`, `o-que-nao-vender`) |
| ⚖️ | Anexar o mapa ao plano de peça; citar dispositivo nas rotas descartadas |

Linha geográfica na proposta 💼: `8 CFR 292.1` — https://www.ecfr.gov/current/title-8/chapter-I/part-292/section-292.1

## O que esta skill **não** faz

- Não inventa processing time, cut-off ou taxa.
- Não substitui o diagnóstico de elegibilidade.
- Não autoriza fraude “porque o cliente tem pressa”.
- Não promete qual rota “o oficial vai gostar”.

## Encadeamento

`diagnostico-de-elegibilidade` → **esta** → `linha-do-tempo-do-caso` (marcos da rota escolhida) → skill C3/C4/C5 → `dossie-pre-protocolo`.

## Guard

1. Sempre as **quatro** dimensões; **reversibilidade** não é opcional.  
2. Explicitar o que **queima a ponte** (negativa por falta de prova, alegação falsa, UP acumulada).  
3. Zero número operacional — só URL.  
4. Sem garantia de resultado/prazo (*Avoid Scams*).  
5. Citar gates C1; não reescrevê-los.
