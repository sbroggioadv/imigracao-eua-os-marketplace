---
name: n400-elegibilidade
description: "Elegibilidade ao Form N-400: via geral de 5 anos (INA 316 / 8 U.S.C. 1427 + 8 CFR 316.2) versus via de 3 anos do cônjuge de cidadão (INA 319(a) / 8 CFR 319.1). Continuous residence, physical presence, GMC, early filing de 90 dias, inglês/civics e Oath. Use quando o LPR pergunta se já pode naturalizar, qual via cabe, ou se o casamento com cidadão encurta o prazo. Não inventa taxa nem processing time — só URL. Encadeia residencia-e-presenca, bom-carater-gmc e teste-civico-2025."
---

# N-400 ELEGIBILIDADE — 5 anos × 3 anos (cônjuge)

> **Camada C6 · Naturalização.** Frentes: 👤 imigrante · ⚖️ advogado.  
> Anexos: `context/anexo-naturalizacao.md` · `context/anexo-ina-estatuto.md`.  
> Gates: `varredura-de-vigencia` (taxa G-1055 no dia) · `trava-de-representacao` (quem pode assinar G-28 no N-400 adjudicado **dentro** dos EUA).

## O que é

O **N-400** (*Application for Naturalization*) pede a cidadania americana a quem já é **LPR** (*lawful permanent resident*). Duas vias principais deste skill:

| Via | Estatuto / reg. | Quem |
|---|---|---|
| **5 anos** (geral) | INA 316 · `8 U.S.C. 1427` · `8 CFR 316.2` | LPR em geral |
| **3 anos** (cônjuge de USC) | INA 319(a) · `8 CFR 319.1` | LPR casado e em *marital union* com cidadão americano |

Form e instruções: https://www.uscis.gov/n-400  
Hub 5 anos: https://www.uscis.gov/citizenship/learn-about-citizenship/citizenship-and-naturalization/i-am-a-lawful-permanent-resident-of-5-years  
Hub 3 anos: https://www.uscis.gov/citizenship/learn-about-citizenship/citizenship-and-naturalization/i-am-married-to-a-us-citizen  
Estatuto: https://uscode.house.gov/view.xhtml?req=granuleid:USC-prelim-title8-section1427  
eCFR Part 316: https://www.ecfr.gov/current/title-8/chapter-I/subchapter-C/part-316  
eCFR Part 319: https://www.ecfr.gov/current/title-8/chapter-I/subchapter-C/part-319

**Ônus da prova:** o applicant ( `8 CFR 316.2(b)` ) — preponderância da evidência. Dossiê **completo antes** de protocolar (TRAVA 2 / PA-2026-05: o oficial pode **negar sem RFE/NOID**).

---

## Via de 5 anos — `8 CFR 316.2(a)` + `8 U.S.C. 1427(a)`

O alien deve estabelecer, em síntese operacional (lista oficial das páginas de cidadania + regulamento):

1. **Idade** ≥ 18 anos no filing.  
2. **LPR** — *lawfully admitted for permanent residence*.  
3. **Continuous residence** nos EUA por **pelo menos 5 anos** após o LPR, até o filing (e continua até a admissão à cidadania — `316.2(a)(6)`).  
4. **Physical presence** de **pelo menos 30 months** nos 5 anos imediatamente anteriores ao filing.  
5. **Jurisdição local:** residiu ≥ **3 months** no State ou *Service district* com jurisdição sobre o local de residência real (imediatamente antes do filing, ou, em *early filing*, antes do exame se a janela de 3 meses cair no período estatutário).  
6. **GMC** (*good moral character*) em todo o período relevante — tipicamente os 5 anos até o Oath (skill `bom-carater-gmc`).  
7. **Apego** aos princípios da Constituição e disposição favorável à ordem dos EUA.  
8. Não ser pessoa descrita em INA 314 (desertores / evasão de serviço militar — ver `316.2(a)(8)`).  
9. **Inglês** (falar/ler/escrever) e **civics** — salvo isenção (skill `teste-civico-2025` + entrevista).  
10. Prestação do **Oath of Allegiance** (skill `entrevista-e-juramento`).

⛔ Continuous residence **≠** physical presence. Detalhe e quebras por viagem: skill `residencia-e-presenca`.

---

## Via de 3 anos — cônjuge de cidadão (`8 CFR 319.1`)

Além de LPR e dos requisitos gerais de naturalização (exceto as faixas de 5 anos substituídas):

| Requisito | Conteúdo |
|---|---|
| Continuous residence | **≥ 3 anos** após LPR (`319.1(a)(2)`) |
| Physical presence | **≥ 18 months** no total (`319.1(a)(4)`) |
| *Marital union* | Vivendo em união marital com o cônjuge **cidadão** pelos **3 anos** que antecedem o **exame** da aplicação; o cônjuge **foi cidadão** durante todo esse período (`319.1(a)(3)`) |
| GMC | Período estatutário de **3 anos** (até o Oath) |
| Jurisdição local | Mesma lógica de 3 months (`319.1(a)(5)`) |
| Continuity pós-filing | Residência contínua dos EUA do filing até a admissão (`319.1(a)(6)`) |

### *Marital union* — o que quebra a via

`8 CFR 319.1(b)`:

- **Divórcio, morte ou expatriação** do cônjuge cidadão **antes** da admissão à cidadania → **inelegível** sob 319(a). Casar de novo com outro cidadão **não** “restaura” a elegibilidade da petição antiga.  
- **Separação legal** quebra a continuidade da união.  
- Separação **informal** = análise caso a caso.  
- Separação **involuntária** (serviço militar, demanda ocupacional essencial) **não** impede, se a união marital permanece.

**Nunca esteve nos EUA:** `319.1(c)` — se o cônjuge alien **nunca** esteve nos EUA, a via 319.1 **não** se estabelece só por união marital no exterior.

**INA 319(b)** (cônjuge de USC em emprego qualificado no exterior): regime **distinto** (sem o mesmo pacote 3 anos/18 meses). Não misturar com 319(a) sem reler a página USCIS e o estatuto no dia.

---

## Early filing — 90 dias de calendário

A página do N-400 permite protocolar até **90 calendar days** **antes** de completar o continuous residence exigido, se a base for:

- LPR de pelo menos 5 anos; **ou**  
- LPR de pelo menos 3 anos **e** casado com cidadão americano.

Fonte: https://www.uscis.gov/n-400  

⛔ Early filing **não** encurta o GMC nem a physical presence: no exame, os requisitos **completos** precisam estar satisfeitos. ⛔ Não protocolar “no escuro” se viagens longas ou GMC estiverem no fio — skill `residencia-e-presenca` e `bom-carater-gmc` primeiro.

---

## O que esta skill **não** resolve sozinha

| Tema | Skill |
|---|---|
| Quebra de residência por viagem / N-470 | `residencia-e-presenca` |
| GMC, voto ilegal, DMV, crime | `bom-carater-gmc` |
| Qual teste cívico (2025 vs 2008) | `teste-civico-2025` |
| Entrevista, Oath, mito da dupla cidadania | `entrevista-e-juramento` |
| N-400 negado | `negativa-n336-i290b` |
| Taxa do N-400 / reduced fee / waiver | **Só** https://www.uscis.gov/g-1055 + página do form no dia (`varredura-de-vigencia`) |
| Quem representa no USCIS | `trava-de-representacao` |

---

## Checklist rápido 👤

```text
[ ] Sou LPR? Desde quando (data do green card / admissão)?
[ ] Via: 5 anos geral OU 3 anos com cônjuge USC + marital union intacta?
[ ] Completei (ou estou a ≤90 dias de) continuous residence da via?
[ ] Physical presence: ≥30 meses (5y) ou ≥18 meses (3y)?
[ ] ≥3 meses no state/district atual?
[ ] Viagens >6 meses / ≥1 ano? → residencia-e-presenca
[ ] Histórico criminal, impostos, pensão, voto, DMV? → bom-carater-gmc
[ ] Estudo civics **2025** (N-400 novo)? → teste-civico-2025
[ ] Dossiê documental completo ANTES de protocolar (TRAVA 2)
```

## Entrega ⚖️

1. Identificar a via e o **dies a quo** do LPR.  
2. Linha do tempo de residência/presença + red flags de abandono.  
3. GMC screen (incluindo checklist eleitoral/DMV).  
4. Só então montar N-400; G-28 **somente** se o representante está na lista de `8 CFR 292.1` aplicável **dentro** dos EUA.  
5. Zero valor em dólar / processing time no corpo da peça de orientação — URL + data da consulta.

## Guard

1. **5 anos** e **3 anos** são vias **distintas**; 3 anos exige união marital + cidadania do cônjuge no período.  
2. Continuous residence ≠ physical presence — nunca “só contar dias”.  
3. Policy Manual **não** é lei (`mapa-normativo-eua`); citar estatuto/CFR e URL.  
4. **Nenhum** fee, cota ou processing time hardcoded — G-1055 e ferramenta de times no dia.  
5. Representação BR: linha geográfica — `trava-de-representacao`.
