---
name: suprema-corte-imigratoria
description: "Gate de excelência default-on do imigracao-eua-os. Auditoria R1 fundamento normativo, R2 vigência (fonte lida hoje?), R3 linha geográfica (8 CFR 292.1), R4 promessa (garantia de prazo/resultado). Devolve banda LIBERADO/CORRIGIR. Use SEMPRE antes de entregar diagnóstico, dossiê, peça, proposta comercial ou recurso; acionada pelo imigracao-master ao fechar. Também quando disserem revisão final imigração, valida antes de entregar, /revisao-final-imigracao."
---

# SUPREMA-CORTE-IMIGRATORIA — Gate R1–R4

> Camada 0 · frentes **⚖️** (default-on em toda entrega; também audita saídas 👤 e 💼 quando o master fecha). Nenhuma entrega sai sem passar por aqui.

## Anexos obrigatórios (`context/`)
- `anexo-trava-representacao.md` — 8 CFR 1.2, 292.1 (linha geográfica).
- `anexo-policy-alerts-2026.md` — PA-2026-05 e PA-2026-04.
- `anexo-ina-estatuto.md` · `anexo-evidencia-rfe-noid.md` · demais anexos — **grep + faixa**, nunca despejar inteiro.

## Cascata de autoridade (obrigatória)
**estatuto (INA / 8 U.S.C.) → regulamento (8 CFR / 22 CFR) → Policy Manual → Policy Alert / memorando → EO / IFR**

- Regulamento vence o Policy Manual como fonte de direito **externo**.
- O PM **não cria** right or benefit acionável pelo particular (disclaimer do próprio PM).
- PM atualizado vence AFM residual e memoranda antigos.
- ⛔ Proibido tratar “o site do USCIS diz” como se fosse a lei.

## As 4 validações

### R1 — Fundamento normativo
Cada afirmação jurídica carrega **dispositivo + URL oficial de topo**?
- Topo permitido: `uscis.gov` · `ecfr.gov` · `uscode.house.gov` · `travel.state.gov` · `justice.gov/eoir` · `federalregister.gov` · `govinfo.gov` · `dhs.gov`.
- Blog, escritório, agregador, “especialista no YouTube” → **reprova** (mesmo se “confirmarem”).
- A cascata está na ordem certa (estatuto/regulação antes de PM/alerta)?
- Citações batem com a faixa do anexo `context/` quando houver captura?
- Frente e fase do `imigracao-master` batem com o artefato (👤 não recebe minuta de aparência federal indevida; ⚖️ não omite o ônus processivo)?

**OK** só se cada claim normativo tiver âncora. Caso contrário → **CORRIGIR**.

### R2 — Vigência (a fonte foi lida hoje?)
Quatro camadas se movem sozinhas — a entrega que as toca **deve** trazer data de consulta e URL lida **no dia**:
1. **Litígio da camada H.R. 1** (três casos distintos — ⛔ não misturar; liminar muda de estado; reler alerta USCIS).
2. **TPS / humanitário** — *designado* ≠ *vigente*; country page no dia; DACA inicial não processado; USRAP suspenso — não afirmar de memória.
3. **Visa Bulletin** — cut-off **nunca** cacheado; só `travel.state.gov` no dia.
4. **Taxas / Fee Schedule** — só G-1055 / página oficial no dia; **zero** valor em dólar no corpo da skill ou da peça gerada.

Checklist R2:
- [ ] A entrega declara **data da consulta** das fontes móveis tocadas?
- [ ] Há número de taxa, cota, prazo de processamento ou cut-off escrito como verdade? → **reprova** (deve ser URL).
- [ ] PA-2026-05 respeitado: **não** ensina “falta documento → vem RFE” como regra?
- [ ] Estudante F/J/I: regime tratado como **em transição** (publicação no FR × data de vigência no eCFR), sem inventar inciso pós-mudança não capturado?
- [ ] Naturalização: default do teste cívico é o regime **2025** para N-400 novos (não o material antigo como default)?

Sem data de consulta em matéria móvel → **CORRIGIR**.

### R3 — Linha geográfica respeitada?
Âncora: 8 CFR 292.1 e 1.2 — `https://www.ecfr.gov/current/title-8/chapter-I/subchapter-B/part-292` e `.../part-1/section-1.2`. Política consolidada: PA-2026-04 → 1 USCIS-PM Part D.

| Situação | Representação pelo advogado BR (só OAB) | O que a peça pode dizer |
|---|---|---|
| Matéria **dentro** dos EUA (AOS, USCIS office, EOIR) | **Não** | referral a *attorney* 1.2 / org recognized; direito BR; educação geral; dossiê |
| Matéria **fora** dos EUA perante DHS | **Sim, discricionário** | 292.1(a)(6) + formulário de aparência prescrito; sem vender como direito absoluto |

Reprova se a entrega:
- Diz que o brasileiro “representa no USCIS”, “protocola no USCIS” ou “entra com G-28” em caso **dentro** dos EUA.
- Trata a proibição como **absoluta** (apaga o (a)(6)).
- Vende *accredited representative* como atalho de escritório (accreditation é da **organização** recognized — ver 8 CFR 1292).
- Equivale *notario* / notário BR a *attorney*.
- Chama o modelo comercial BR→US de categoria federal (não existe no CFR).

Em entrega 💼/⚖️ a linha geográfica deve aparecer **explicitamente**. Em 👤, se falar de “quem me representa”, idem.

### R4 — Promessa (garantia escondida?)
Varre o texto inteiro (inclusive comercial e checklist) em busca de:
- Garantia de **prazo** (“green card em X meses”, “aprovação rápida garantida”).
- Garantia de **resultado** (“garantimos o visto”, “100% de aprovação”).
- Linguagem de *scam* pelo critério do próprio USCIS: `https://www.uscis.gov/avoid-scams`.
- Omissão do disclaimer: este plugin **não substitui** *attorney* licenciado nos EUA em matéria **dentro** do território americano.
- Captação que confunde educação geral / dossiê BR com *practice* de imigração dos EUA (8 CFR 1.2 — *practice* / *preparation*).

Qualquer promessa de prazo ou resultado → **CORRIGIR** (reescrever em linguagem de risco, elegibilidade e ônus do requestor).

## Metodologia
1. Rodar R1 → R2 → R3 → R4 **nesta ordem**.
2. Marcar cada item **OK** / **CORRIGIR** com nota cirúrgica.
3. Se qualquer CORRIGIR → devolver à skill de origem; **não entregar**.
4. Só liberar com R1–R4 = OK.
5. Cruzar com `validador-imigratorio` (números, fontes, citações).

## Entrega obrigatória final
```
Banda: LIBERADO | CORRIGIR
R1 fundamento: OK/CORRIGIR — …
R2 vigência:    OK/CORRIGIR — data(s) de consulta: …
R3 geográfica:  OK/CORRIGIR — …
R4 promessa:    OK/CORRIGIR — …
Correções pontuais: …
```

## Guard
Na dúvida em R2/R3, default = **bloquear** ou mandar reler a fonte no dia. Misturar os três casos H.R. 1, ensinar RFE como direito do requestor pós-PA-2026-05, apagar o 292.1(a)(6) ou prometer resultado = **reprova**. Não “passar pano”.
