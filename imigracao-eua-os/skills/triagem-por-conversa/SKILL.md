---
name: triagem-por-conversa
description: "Triagem conversacional do caso de imigração EUA. Abre por 'o que te faz querer ir, e qual é o seu prazo?'; usa botões; ramifica em trilhas (não-imigrante, green card, humanitário, comercial, contencioso). Nunca promete resultado nem prazo de governo. Se pedirem garantia, cita Avoid Scams do USCIS. Use após onboarding, quando o master precisa classificar frente+fase+trilha, ou quando o usuário chega com pedido vago."
---

> **🖱️ Escolhas = botões:** nas perguntas de **lista fechada** use **AskUserQuestion** (máx. 4 opções; se houver mais, divida). Não peça para digitar 1/2/3.

# TRIAGEM-POR-CONVERSA — o que te faz querer ir?

> **Camada C2 · Triagem e diagnóstico.** Frentes: 👤 imigrante · 💼 comercial · ⚖️ advogado.  
> Não escolhe a categoria final sozinha — **abre** a conversa, grava fatos e **encaminha**.  
> Gates: se a resposta tocar taxa/fila/TPS/H.R.1 → `varredura-de-vigencia`. Se 💼/⚖️ for entregar serviço → `trava-de-representacao`.  
> Anexos: `context/anexo-ina-estatuto.md` · `context/anexo-nao-imigrante.md`.

## ⛔ Anti-scam e anti-promessa (inviolável)

- **Nunca** prometa resultado (aprovação, green card, visto) **nem** prazo de processamento do governo.
- Se a pessoa pedir **garantia**, **prazo fixo** ou "só me garante que passa":
  1. Explicar que **ninguém honesto** garante resultado em imigração — o adjudicator decide com base no dossiê e na lei.
  2. Citar o critério do próprio USCIS em *Avoid Scams*: https://www.uscis.gov/avoid-scams  
  3. Redirecionar para diagnóstico real + dossiê completo (TRAVA 2 / PA-2026-05).
- Taxa, cota, cut-off e *processing time* → **só URL + leitura no dia** (TRAVA 3). Nunca número de memória.

## Pergunta-âncora (sempre primeiro, aberta)

Perguntar em texto livre (não botão):

> **"O que te faz querer ir, e qual é o seu prazo?"**

Capturar em 1–3 frases: **motivo** (família, estudo, trabalho, investimento, proteção, negócio do escritório) e **urgência subjetiva** (exploração / marco pessoal / prazo de governo no notice / risco).  
A urgência **não** autoriza inventar dias de processamento.

---

## Bloco A — Onde está e em que status (botões)

| Opção | Significado | Handoff imediato |
|---|---|---|
| **Fora dos EUA** (Brasil ou terceiro país) | Via consular / petição a partir do exterior | `imigrante-x-nao-imigrante` → elegibilidade |
| **Nos EUA em status** | Admissão/extensão válida | Manutenção de status `8 CFR 214` + cuidado com *overstay* |
| **Nos EUA fora de status** | ⛔ não minimizar | **Antes de qualquer rota otimista:** `barras-3-10-anos` + `diagnostico-de-elegibilidade` (pergunta de *unlawful presence*) |
| **Não sei classificar** | Fatos faltando | Coletar entrada, visto, I-94, pendências — **sem** chutar |

Regulamento de manutenção de status: https://www.ecfr.gov/current/title-8/chapter-I/part-214  
Estatuto de admissão de não-imigrantes: `8 U.S.C. 1184` — https://uscode.house.gov/view.xhtml?req=granuleid:USC-prelim-title8-section1184

---

## Bloco B — Trilha de vida (botões; até 4 por rodada)

Depois do âncora, classificar o **projeto**:

1. **Temporário com retorno** (turismo, negócio curto, estudo com laços no exterior) → C3 não-imigrante; atenção a **INA 214(b)** / `8 U.S.C. 1184(b)`.
2. **Permanecer / morar** (família, emprego, investimento, DV) → C4 green card; inadmissibilidade `8 U.S.C. 1182`.
3. **Proteção / humanitário** (asilo, TPS, U/T/VAWA, parole…) → C5; TPS = *designado* ≠ *vigente* → `varredura-de-vigencia` + country page no dia.
4. **Já tenho processo / notice / RFE / NTA** → fase = contencioso ou resposta; ⚖️ + representação se inland.

Bifurcação fundadora: skill `imigrante-x-nao-imigrante`.  
Classes não-imigrante: `8 U.S.C. 1101(a)(15)` — https://uscode.house.gov/view.xhtml?req=granuleid:USC-prelim-title8-section1101

---

## Bloco C — Frente de quem fala (se ainda não gravada)

Botões alinhados ao onboarding:

- 👤 **Imigrante** — "o que eu faço / como monto?"
- 💼 **Comercial** — "como vendo / contrato / rede"
- ⚖️ **Advogado** — "como monto a peça / o recurso"

Se 💼 ou ⚖️: **GATE 2** `trava-de-representacao` antes de proposta, G-28/G-28I ou frase de "representar no USCIS". Linha geográfica: `8 CFR 292.1(a)(6)` — https://www.ecfr.gov/current/title-8/chapter-I/part-292/section-292.1

---

## Bloco D — Fatos mínimos (só o que destrava a trilha)

Perguntar o necessário, em botões ou texto curto — **sem** colher PII sensível em artefato compartilhado (A-Number, passaporte completo, e-mail):

| Fato | Por que importa |
|---|---|
| Nacionalidade / país de residência | Cota, DV, tratados E, TPS |
| Parente cidadão/LPR nos EUA? grau | IR × preferências F |
| Emprego/oferta/empresa multinacional? | H/L/O/EB |
| Já esteve nos EUA? *overstay* / deportação / remoção? | **Obrigatório** antes de recomendar — `diagnostico-de-elegibilidade` + `barras-3-10-anos` |
| Petição já protocolada? formulário? | Fase = fila / RFE / AOS vs consular |
| Menor emigrando? | `menor-emigrante` + ECA (ponte BR) |

Se **qualquer** indício de estadia irregular, entrada sem inspeção, ou saída após *unlawful presence*: **parar o mapa otimista** e abrir o diagnóstico de elegibilidade com a pergunta de status primeiro.

---

## Ramificação → skills (após gravar perfil)

| Trilha gravada | Próximo |
|---|---|
| Motivo + status claros, sem barra óbvia | `diagnostico-de-elegibilidade` |
| Duas+ rotas plausíveis | `mapa-de-caminhos` (tempo · custo · risco · **reversibilidade**) |
| Já em fila / marcos | `linha-do-tempo-do-caso` |
| Categoria específica (B, F, H, IR, EB…) | skill C3/C4/C5 correspondente |
| Montar pacote | `dossie-pre-protocolo` (TRAVA 2 — negativa sem RFE desde PA-2026-05) |
| Captação / proposta | C7 + `captacao-honesta` / `o-que-nao-vender` |

PA-2026-05 (evidência / RFE / NOID): https://www.uscis.gov/sites/default/files/document/policy-manual-updates/20260805-EvidentiaryStandards.pdf

---

## Saída obrigatória da triagem

Gravar em 5–10 linhas (sem PII):

```text
## Perfil de triagem
- Motivo (âncora): …
- Prazo subjetivo: exploração | marco pessoal | notice de governo | risco
- Situação: fora dos EUA | EUA em status | EUA fora de status | indefinida
- Trilha: não-imigrante | imigrante/LPR | humanitário | mista | contencioso
- Frente: 👤 | 💼 | ⚖️
- Flags: FORA_DE_STATUS? | POSSIVEL_UNLAWFUL_PRESENCE? | MENOR? | NOTICE?
- Handoff: <skill>
- Anti-promessa: sem garantia de resultado/prazo (Avoid Scams)
```

## O que esta skill **não** faz

- Não fecha elegibilidade sozinha.
- Não redige DS-160, I-130, I-485, G-28.
- Não calcula dias de *unlawful presence*.
- Não cotiza honorário nem taxa governamental.
- Não trata Policy Manual como lei (`mapa-normativo-eua`).

## Guard

1. Abre sempre pelo âncora de motivo + prazo subjetivo.  
2. Botões em listas fechadas.  
3. Zero promessa de resultado ou de prazo de governo; *Avoid Scams* se pedirem garantia.  
4. Fora de status → não minimizar; aponta barras.  
5. Zero número operacional (taxa/cota/cut-off/processing) — só URL.  
6. Encadeia gates C1; não reescreve `trava-de-representacao` nem `varredura-de-vigencia`.
