---
name: dossie-pre-protocolo
description: "Espinha do produto (TRAVA 2). Monta o checklist de prova inicial ANTES de protocolar, lendo as instruções oficiais do formulário. Desde 05/08/2026 (PA-2026-05) o USCIS restaurou a discricionariedade de negar sem RFE e sem NOID por falta de initial evidence — inclusive pedidos já pendentes. 'Se faltar documento vem RFE' é conselho de risco. Use quando o cliente ou o escritório for protocolar qualquer benefit request, vender pacote completo de primeira, ou auditar se o dossiê está pronto. Serve às 3 frentes."
---

# DOSSIÊ-PRÉ-PROTOCOLO ⭐⭐ — a espinha do produto

> **Camada transversal · TRAVA 2.** Frentes: 👤 imigrante · 💼 comercial · ⚖️ advogado.  
> Anexos: `context/anexo-policy-alerts-2026.md` (PA-2026-05) · `context/anexo-evidencia-rfe-noid.md` (8 CFR 103.2, 103.8).  
> Gates: roda **depois** de `varredura-de-vigencia` (se tocar taxa/litígio) e `trava-de-representacao` (se for entrega 💼/⚖️).

## Por que esta skill existe

Desde **05/08/2026**, Policy Alert **PA-2026-05** (*Evidence, Requests for Evidence, and Notices of Intent to Deny*), o USCIS **restaurou** a discricionariedade dos oficiais de **negar sem RFE e sem NOID** quando falta *initial evidence* ou o pedido não demonstra elegibilidade — com efeito **imediato** sobre pedidos **pendentes ou protocolados em/após** essa data.

PDF oficial: https://www.uscis.gov/sites/default/files/document/policy-manual-updates/20260805-EvidentiaryStandards.pdf  
Alerta: https://www.uscis.gov/newsroom/alerts/uscis-to-reduce-frivolous-immigration-benefits-requests-by-reinforcing-evidence-standards

Verbatim do Policy Alert:

> "Accordingly, USCIS is updating its policy guidance to restore USCIS officers' **full discretion to deny such benefit requests without first issuing an RFE or NOID**, as allowed by the regulations."

### A nuance que **não** pode se perder

O regulamento **`8 CFR 103.2(b)(8)(ii)`** **sempre** permitiu negar direto por falta de *initial evidence*. O que mudou em 05/08/2026 foi a **instrução interna** (policy guidance): a política **anterior** mandava o oficial **preferir** emitir RFE/NOID; a nova **devolve** a discricionariedade plena de negar sem esse passo intermediário.

Fonte do regulamento: https://www.ecfr.gov/current/title-8/chapter-I/part-103/section-103.2

⛔ **Proibido** ensinar: *"se faltar documento, o USCIS pede por RFE."* Essa frase virou **conselho de risco** em 05/08/2026.

✅ **O produto vende e executa:** dossiê **completo** de prova inicial **antes** de protocolar.

Exceção de regime: asilo e refúgio têm regras próprias de RFE/NOID (nota 5 do PA-2026-05). Não generalizar.

---

## Base regulatória (o ônus é do pedido)

| Dispositivo | Conteúdo operacional | URL |
|---|---|---|
| `8 CFR 103.2(b)(1)` | Elegibilidade **no filing** e até a adjudicação; pedido completo com **toda** *initial evidence* exigida por regulamento e **instruções do form** | https://www.ecfr.gov/current/title-8/chapter-I/part-103/section-103.2 |
| `8 CFR 103.2(b)(8)(ii)` | Sem *initial evidence* completa ou sem elegibilidade: USCIS **pode negar** ou pedir o que falta (discricionário) | idem |
| `8 CFR 103.2(b)(8)(iii)` | Com *initial evidence* mas sem elegibilidade: negar, RFE de prova adicional, **ou** NOID | idem |
| `8 CFR 103.2(a)(1)` | Form executado **conforme form instructions** | idem |
| INA 291 / ônus da prova | O *requestor* carrega o ônus (citado no PA-2026-05) | https://uscode.house.gov/ |

Policy Manual **obriga o oficial**, **não** cria direito acionável (TRAVA 8). Cascata: estatuto → 8 CFR → PM → PA.

---

## Protocolo (ordem fixa — nunca pular)

1. **Identificar o form** (I-130, I-485, I-129, N-400, I-589…).  
2. **Abrir a página oficial do form** em https://www.uscis.gov e as **form instructions** vigentes (PDF/página do dia).  
3. **Extrair a lista de *initial evidence*** literal das instruções + o que o 8 CFR da categoria exigir.  
4. **Cruzar com a ponte Brasil** quando o fato nasceu no BR:
   - `cadeia-documental-br` (certidões, validade, o que o consulado pede)
   - `apostila-de-haia` (documento público BR → exterior)
   - `traducao-publica` (⛔ juramentada BR ≠ certificação USCIS — ver skill)
   - `menor-emigrante` se houver menor
5. **Classificar cada item:**  
   - ✅ nos autos / na pasta  
   - 🟡 existe mas fraco (secundário, affidavit, lacuna de tradução)  
   - ⛔ ausente  
6. **Gate de protocolo:** se houver ⛔ de *initial evidence* **obrigatória** → **não protocolar**. Diz o gap e o que falta.  
7. **Registrar na saída** a data da leitura das instruções e a URL do form.

### Formato de saída obrigatório

```text
## Dossiê pré-protocolo
- Form: <código>
- URL instruções: <uscis.gov/...>
- Data da leitura: AAAA-MM-DD
- Initial evidence (checklist):
  - [ ] item — status ✅/🟡/⛔ — fonte (instrução § / 8 CFR)
- Gaps bloqueantes: …
- Decisão: PRONTO PARA PROTOCOLAR | NÃO PROTOCOLAR
- Aviso TRAVA 2: negativa sem RFE/NOID é discricionária desde 05/08/2026 (PA-2026-05)
```

---

## As 3 frentes

| Frente | O que esta skill entrega |
|---|---|
| 👤 **Imigrante** | Entende **por quê** o pacote tem de estar completo **antes** do filing; checklist legível; não confia em "depois o USCIS pede" |
| 💼 **Comercial** | Vende **exatamente** o pacote completo de primeira — núcleo honesto do serviço BR (dossiê + ponte documental + referral). Não vende "placeholder filing" |
| ⚖️ **Advogado** | Monta o pacote: mapeia *initial* vs *additional* evidence, indexa exhibits, confere assinatura/fee/instruções; se for só-OAB inland, **não** assina como G-28 — orquestra com *attorney* US (`trava-de-representacao`) |

---

## O que **não** entra neste dossiê (e para onde mandar)

| Tema | Skill / regra |
|---|---|
| Responder RFE/NOID já emitidos | `resposta-a-rfe-noid` (prazo = **teto**; correio +3, não +14) |
| Taxa em dólar | só URL do G-1055 no dia — `varredura-de-vigencia` · https://www.uscis.gov/g-1055 |
| Cut-off / Visa Bulletin | URL do mês · `varredura-de-vigencia` |
| Representação perante o DHS | `trava-de-representacao` — linha **geográfica** |
| Prova de DNA / vínculo familiar | PA de DNA evidence (mesmo dia 05/08/2026) — ler PDF oficial antes de afirmar |

---

## Guard (inviolável)

1. **Nunca** escrever que o USCIS "sempre emite RFE" se faltar documento.  
2. Sempre explicar a nuance: regulamento **sempre** permitia negar; em 05/08/2026 mudou a **política interna** (PA-2026-05).  
3. Checklist de *initial evidence* **só** das instruções oficiais do form + 8 CFR — **nunca** inventar lista universal.  
4. Zero taxa, cota, processing time ou cut-off hardcoded — só URL + data.  
5. Policy Manual / Policy Alert **não** são lei (TRAVA 8).  
6. Asilo/refúgio: não generalizar o regime de RFE/NOID do 103.2.  
7. Entrega 💼/⚖️ passa por `trava-de-representacao`.
