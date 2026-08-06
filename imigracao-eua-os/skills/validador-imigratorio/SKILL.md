---
name: validador-imigratorio
description: "Anti-alucinação do imigracao-eua-os. Bloqueia saída com valor em dólar, cota, prazo de processamento ou cut-off do Visa Bulletin como número; citação sem dispositivo; fonte fora do topo (só uscis/ecfr/uscode/travel.state/justice.gov/eoir/federalregister/govinfo/dhs). Blog e escritório não confirmam. Use antes de selar qualquer entrega, ou quando disserem confere as citações, pode protocolar, valida números."
---

# VALIDADOR-IMIGRATORIO — Anti-alucinação

> Camada 0 · frentes **👤 💼 ⚖️**. **Não redige:** audita item a item. A Suprema Corte julga excelência (R1–R4); **aqui** a trava dura de número, citação e fonte.

## Anexos obrigatórios (`context/`)
Todos sob demanda — **grep o dispositivo e leia a faixa**:
`anexo-trava-representacao.md` · `anexo-policy-alerts-2026.md` · `anexo-evidencia-rfe-noid.md` · `anexo-nao-imigrante.md` · `anexo-green-card.md` · `anexo-humanitario-inadmissibilidade.md` · `anexo-naturalizacao.md` · `anexo-ina-estatuto.md`.

## Objetivo
Para cada afirmação: **CONFIRMADO** · **CORRIGIR → [substituto]** · **CHECAR AO VIVO** (fonte móvel / gap do corpus). Um item bloqueante pendente → **não selar**.

## Fontes de topo (whitelist fechada)
| Domínio | Uso |
|---|---|
| `uscis.gov` | formulários, Policy Manual, Policy Alerts, fee schedule |
| `ecfr.gov` | 8 CFR / 22 CFR vigente |
| `uscode.house.gov` | INA / 8 U.S.C. |
| `travel.state.gov` | Visa Bulletin, consular |
| `justice.gov/eoir` | immigration court / BIA |
| `federalregister.gov` | regras finais, IFR |
| `govinfo.gov` | espelho GPO |
| `dhs.gov` | componentes DHS |

⛔ **Blog, escritório de advocacia, agregador, rede social, Wikipedia, “segundo especialistas”** — **não são fonte**, nem para “confirmar”. Se a única âncora for essa → **CORRIGIR** ou **CHECAR AO VIVO** na whitelist.

## Bloqueios absolutos (a saída inteira cai)

### 1. Número operacional no corpo
Bloqueia se encontrar, escrito como verdade (não como nome de formulário nem como URL):
- **Valor em dólar** de taxa, investimento, multa ou “custo do processo”.
- **Cota** numérica anual (ex.: teto de categoria) como número fixo na peça.
- **Prazo de processamento** (“demora X meses”, “aprovação em Y semanas”) como fato.
- **Cut-off do Visa Bulletin** (datas de prioridade) como número/data cacheada.

**Correção obrigatória:** substituir pelo **URL oficial** e a ordem “consultar na data de hoje; devolver a data da consulta”.
- Taxas: página Fee Schedule / G-1055 no `uscis.gov`.
- Visa Bulletin: `https://travel.state.gov/content/travel/en/legal/visa-law0/visa-bulletin.html`
- Processing times: ferramenta oficial USCIS de processing times (URL da página vigente).

Exceções que **não** disparam o bloqueio:
- Número de **dispositivo** (ex.: 8 CFR 292.1(a)(6), INA 212(a)).
- Número de **formulário** (I-130, N-400, G-28I).
- Número de **Policy Alert** / docket / FR (PA-2026-05, 91 FR …).
- Data de **publicação ou vigência de ato normativo** com URL (ex.: data do PA, data efetiva de final rule) — desde que não seja “seu caso sai em X dias”.

### 2. Citação sem dispositivo
Toda afirmação normativa precisa de:
1. **Dispositivo** (seção do INA / 8 U.S.C. / 8 CFR / 22 CFR) **ou** identificação inequívoca do Policy Alert/PM com volume-parte-capítulo; **e**
2. **URL oficial** da whitelist.

“Segundo o USCIS”, “a lei americana manda”, “em geral o consulado exige” sem âncora → **CORRIGIR**.

### 3. Fonte fora do topo
Mesmo com URL, se o host não está na whitelist → **reprova**. Não “passar” porque o blog cita o CFR — ir ao eCFR.

## Tabela de correções travadas (régua do produto)

| Nunca escreva | Escreva / faça |
|---|---|
| 1. Valor de taxa/cota/cut-off/prazo de fila no corpo | URL oficial + “ler no dia” + data da consulta |
| 2. “Se faltar documento, o USCIS pede RFE” | PA-2026-05: oficial pode **negar sem RFE/NOID**; ônus no requestor (8 CFR 103.2(b)); dossiê completo antes de protocolar · PDF: `https://www.uscis.gov/sites/default/files/document/policy-manual-updates/20260805-EvidentiaryStandards.pdf` |
| 3. Acréscimo postal internacional antigo (além do regulamento) | Só o acréscimo de correio em 8 CFR 103.8(b) — reler eCFR no dia; a política antiga de acréscimo internacional extra **acabou** no PA-2026-05 |
| 4. “Prazo de RFE = o máximo regulatório como se fosse padrão” | 8 CFR 103.2(b)(8)(iv): o regulamento fixa **teto**, não padrão — ler o notice |
| 5. “Advogado BR representa no USCIS / protocola / G-28” (dentro dos EUA) | Dentro: **não** (lista 292.1(a)(1)–(5)). Fora: 292.1(a)(6) discricionário + aparência prescrita · `https://www.ecfr.gov/current/title-8/chapter-I/subchapter-B/part-292` |
| 6. Proibição de representação BR como **absoluta** | Existe a faixa (a)(6); não apagar |
| 7. *Accredited rep* como produto de escritório | Accreditation da **organização** recognized (8 CFR 1292); não há rep autônomo de imigração “avulso” no federal |
| 8. Modelo comercial BR→US como “licença federal” | Não existe categoria CFR; é arquitetura de compliance (direito BR + educação + dossiê + referral) |
| 9. *Notario* / notário BR = attorney | 8 CFR 1.2 define *attorney*; USCIS *Avoid Scams* |
| 10. “Garantimos o visto / green card / prazo” | Proibido; linguagem de risco + ônus do requestor |
| 11. Pagamento H-1B da camada H.R. 1 “em vigor” **ou** “morto” | Estado: **vacatado sob apelação** — reler alerta USCIS no dia; não misturar os três casos judiciais |
| 12. TPS de país “designado” como vigente | Country page no dia; designado ≠ vigente |
| 13. DACA **inicial** como obtenível | Renovações processadas; iniciais aceitas mas **não** processadas (ordem judicial) — confirmar página USCIS no dia |
| 14. USRAP / refúgio como programa normal | USRAP suspenso (EO); confirmar página USCIS no dia |
| 15. Teste cívico default 2008 (100/10/6) | Default vigente para N-400 novos = regime **2025** — página *Naturalization Interview and Test* no uscis.gov |
| 16. EB-5 com narrativa antiga de patamares | Usar página *About EB-5* vigente (RIA); **nunca** hardcodar o valor — URL |
| 17. “O Policy Manual manda, logo é a lei” | PM não cria right acionável; cascata estatuto→CFR→PM→alerta |
| 18. Verbatim de estatuto “de memória” | Grep em `anexo-ina-estatuto.md` / uscode; sem hit → CHECAR AO VIVO |

## 🟡 / GAP — nunca afirmar seco
Itens do corpus em gap (não viram fato categórico):
- Faixas verbatim de estatuto/regulação não capturadas no anexo.
- Regulatory text completo dos novos 214.2(f)/(j)/(i) pós-transição.
- Valores de fees não no G-1055 lido no dia.
- CSPA, PERM/DOL, public charge 2026, cancellation 42A/42B — sem captura dedicada.
- UPL estadual (CA/NY/FL/TX…): tabela por estado ausente → não generalizar.

**Régua do 🟡:** afirma o provado → marca o que falta → diz o que conferir na whitelist → roteia. Nunca vira categórico.

## Metodologia
1. Extrair **todo** número, citação, URL e promessa do rascunho.
2. Rodar os **bloqueios absolutos** (dólar/cota/prazo-processamento/cut-off; citação sem dispositivo; fonte fora do topo).
3. Rodar a **tabela de correções** + lista 🟡/GAP.
4. Grep no anexo quando houver captura; comparar redação.
5. Veredito por item + global.

## Entrega obrigatória final
Tabela:

| Item | Tipo (nº/citação/fonte/promessa) | Veredito | Nota |
|---|---|---|---|
| … | … | CONFIRMADO / CORRIGIR / CHECAR AO VIVO | … |

Global: **PODE SELAR** só com zero CORRIGIR e zero CHECAR pendente bloqueante. Senão → devolve à skill de origem.

## Guard
Nenhuma entrega de imigração sela com número operacional solto, citação órfã ou fonte de blog. Fonte em `context/` + whitelist vence memória do modelo. A Suprema Corte (R1–R4) roda em paralelo no fecho; este validador é a **trava de alucinação**.
