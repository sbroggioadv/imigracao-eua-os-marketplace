---
name: mapa-normativo-eua
description: "Cascata de autoridade do direito de imigração dos EUA: estatuto (INA/8 U.S.C.) → regulamento (8 CFR/22 CFR) → USCIS Policy Manual → Policy Alert/memorando → EO/IFR. O Policy Manual não é lei e não cria direito acionável pelo particular. Use antes de citar 'o site do USCIS', redigir peça, ranquear fontes, ou quando houver conflito entre manual, alerta e regulamento. Nunca eleva página web a estatuto."
---

# MAPA-NORMATIVO-EUA — cascata de autoridade

> **Camada C1 · Fundação.** Frentes: ⚖️ advogado (principal) · 👤/💼 quando a pessoa pergunta "isso é lei ou política?".  
> Materializa a **TRAVA 8** do corpus: o Policy Manual **não é lei**.  
> Anexos: `context/anexo-ina-estatuto.md` · `context/anexo-trava-representacao.md` · `context/anexo-policy-alerts-2026.md`.

## A cascata (ordem obrigatória de citação)

```text
1. Estatuto — INA / 8 U.S.C.  (+ emendas: Pub. L., inclusive Pub. L. 119-21 / H.R. 1)
2. Regulamento — 8 CFR (DHS) e 22 CFR (Department of State), eCFR atual
3. USCIS Policy Manual (e, no DOS, 9 FAM como política consular)
4. Policy Alert / memorando / guidance que atualiza o Manual ou o AFM residual
5. Executive Order / Interim Final Rule / Final Rule (Federal Register) — com data de efeito
```

**Regra de prevalência entre camadas:**

| Conflito | Quem vence (para o particular / para a peça) |
|---|---|
| Regulamento × Policy Manual | **Regulamento** como fonte de direito **externo** |
| Policy Manual atualizado × memorando/AFM antigo | **Manual atualizado** (e o PA que o altera) para o **oficial** USCIS |
| Estatuto × tudo abaixo | **Estatuto** vence quando o regulamento/PM não puder contrariá-lo — cascata corpus-bound: estatuto → regulamento → PM → alerta; **nunca** esconder o texto estatutário |
| Página de marketing do USCIS × eCFR | **eCFR / U.S. Code** |

⛔ **Proibido** escrever *"segundo o site do USCIS"* como se fosse a lei. Forma correta: *"segundo o 8 CFR … (eCFR); o Policy Manual Vol. … orienta o oficial; alerta PA-… de [data] alterou a orientação."*

## O que cada degrau é (e não é)

### 1. Estatuto — INA / 8 U.S.C.

- Lei federal de imigração e nacionalidade.
- Leitura: https://uscode.house.gov/ (edição *prelim* corrente) · captura GPO no anexo: `context/anexo-ina-estatuto.md`.
- ⚠️ A edição anual impressa pode **atrasar** emendas (ex.: Pub. L. 119-21). Para texto corrente: *House OLRC* +, na prática, o regulamento e o form instruction que implementam.
- Exemplos de âncora do produto: `8 U.S.C. 1101` (definições, classes de não-imigrante em 1101(a)(15)) · `1182` (inadmissibilidade) · `1184` (admissão de não-imigrantes, incl. presunção 214(b)) · `1255` (ajuste) · `1362` (right to counsel).

### 2. Regulamento — 8 CFR / 22 CFR

- Tem força de **regra vinculante** publicada no Federal Register e codificada.
- **8 CFR**: DHS (USCIS, CBP, ICE no que couber) + chapter V (EOIR/DOJ) em partes 1000+.
- **22 CFR**: vistos e prática consular (DOS).
- Leitura viva: https://www.ecfr.gov/ · Federal Register: https://www.federalregister.gov/
- Anexos do plugin trazem faixas verbatim de representação, evidência, não-imigrante, green card, humanitário, naturalização — **preferir o anexo + eCFR** a parafrasear de memória.

### 3. USCIS Policy Manual

- Orienta o **oficial** do USCIS na adjudicação.
- Disclaimer do próprio Manual (TRAVA 8 / corpus): **não** cria *substantive or procedural right or benefit* acionável pelo particular.
- URL hub: https://www.uscis.gov/policy-manual
- Uso correto na peça: *"o oficial está instruído a … (cite volume/part/chapter)"* — não *"o Manual me confere o direito a …"*.
- **9 FAM** (DOS): política consular; tratar como política, com `22 CFR` como regulamento. Não há, no corpus, disclaimer idêntico ao do PM capturado — não inventar simetria perfeita.

### 4. Policy Alert / memorando

- Atualiza o Manual com data de efeito; supersede AFM/memos antigos quando o PA diz que supersede.
- Exemplos âncora 2026 (anexo `anexo-policy-alerts-2026.md`):
  - **PA-2026-05** (evidência / RFE / NOID) — https://www.uscis.gov/sites/default/files/document/policy-manual-updates/20260805-EvidentiaryStandards.pdf · alerta: https://www.uscis.gov/newsroom/alerts/uscis-to-reduce-frivolous-immigration-benefits-requests-by-reinforcing-evidence-standards
  - **PA-2026-04** (attorneys and representatives; `1 USCIS-PM Part D`) — https://www.uscis.gov/sites/default/files/document/policy-manual-updates/20260713-AttorneysAndRepresentatives.pdf
- Policy Alert **não derroga** o 8 CFR: realinha a **política** ao regulamento (como o PA-2026-05 declara fazer com `8 CFR 103.2(b)(8)` e `103.8(b)`).

### 5. EO / IFR / Final Rule

- Ato do executivo ou regra com efeito em data certa (ex.: final rules no FR que alteram `8 CFR 214` etc.).
- Sempre: número do FR, RIN se houver, **data de efeito**, e se há *stay*/vacatur judicial (aí entra `varredura-de-vigencia`).
- FR: https://www.federalregister.gov/ · govinfo: https://www.govinfo.gov/

## Como citar (padrão do plugin)

Toda afirmação normativa na saída deve carregar **dispositivo + URL oficial**:

```text
[camada] dispositivo — URL
Ex.: Regulamento: 8 CFR 292.1(a)(6) — https://www.ecfr.gov/current/title-8/chapter-I/part-292/section-292.1
Ex.: Estatuto: 8 U.S.C. 1184(b) — https://uscode.house.gov/view.xhtml?req=granuleid:USC-prelim-title8-section1184
Ex.: Política: 1 USCIS-PM E.6 (via PA-2026-05) — PDF do PA acima
```

Ordem na peça administrativa: **estatuto → regulamento → (se útil) Manual/PA**. Não abrir com "o site diz".

## Conflitos e liminares

- Liminar federal pode **vacatar** guidance ou suspender policy sem apagar o estatuto. Estado processual = **camada móvel** → `varredura-de-vigencia` + alerta USCIS do dia.
- Não misturar "a lei caiu" com "o guidance X foi vacatado".
- IFR da Pub. L. 119-21 e fees associados: ler G-1055 e alertas no dia — **zero** valor em dólar hardcoded nesta skill.

## Formulários e *form instructions*

- `8 CFR 1.2` define que *form instructions* no site oficial do componente contam como versão aplicável.
- Instrução de form **não** vira estatuto; descumprir pode matar *proper filing* sob `8 CFR 103.2`.
- Forms: https://www.uscis.gov/forms

## Checklist rápido antes de publicar uma frase

1. Achei o **dispositivo** (seção U.S.C. ou CFR)? Se só "o USCIS recomenda" → rebaixar a política e achar o CFR/INA.
2. O Manual está sendo vendido como **direito do particular**? → corrigir.
3. Há PA mais novo que o treino? → `varredura-de-vigencia` + PDF do PA.
4. Há litígio sobre o guidance? → não afirmar vigência plena sem alerta do dia.
5. Estou citando taxa/cota/cut-off? → só URL (`g-1055`, Visa Bulletin), nunca número de memória.

## Encadeamento

- Com `trava-de-representacao`: representação é **regra** (`292.1` / `1.2`), não "política do site".
- Com `quem-e-quem`: cada órgão aplica trechos diferentes da cascata (DOS consular · USCIS benefício · EOIR *removal*).
- Com `validador-imigratorio` / `suprema-corte-imigratoria`: auditoria de citação na ordem da cascata.

## Guard

1. Cascata **sempre** na ordem estatuto → regulamento → PM → alerta → EO/IFR.
2. PM **não** cria direito acionável pelo particular.
3. Regulamento vence PM como direito externo.
4. Nunca "o site do USCIS = a lei".
5. Zero número operacional (taxa/cota/cut-off) no corpo — só URL.
