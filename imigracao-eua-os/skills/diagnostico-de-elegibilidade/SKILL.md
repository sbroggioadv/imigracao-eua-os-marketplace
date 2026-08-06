---
name: diagnostico-de-elegibilidade
description: "Diagnostica quais categorias de imigração EUA a pessoa realmente alcança e quais estão fechadas no caso concreto. Antes de qualquer recomendação, pergunta se já esteve fora de status nos EUA (unlawful presence) e aponta barras-3-10-anos. Cruza 214(b), inadmissibilidade 212(a), status e base (família/emprego/estudo). Use após triagem, quando pedirem 'qual visto serve pra mim' ou para filtrar rotas impossíveis."
---

# DIAGNÓSTICO-DE-ELEGIBILIDADE — o que realmente se alcança

> **Camada C2 · Triagem e diagnóstico.** Frentes: 👤 imigrante · ⚖️ advogado  
> (💼 usa o resultado para proposta honesta — não inventa categoria “vendável”.)  
> Anexos: `context/anexo-ina-estatuto.md` · `context/anexo-nao-imigrante.md`.  
> Gates: `varredura-de-vigencia` se tocar TPS/taxas/Visa Bulletin/H.R.1; `trava-de-representacao` se ⚖️ for montar peça inland.

## ⛔ Gate zero — *fora de status* antes de qualquer recomendação

**Antes** de sugerir B, F, H, IR, EB, asilo, ajuste ou “só protocola”:

> **"Você já esteve nos EUA fora de status — sem autorização válida, *overstay*, entrada sem inspeção, ou com ordem de remoção?"**

| Resposta | Ação |
|---|---|
| **Sim** / **não sei** / indícios | ⛔ **Não** recomendar rota ainda. Abrir **`barras-3-10-anos`** (*unlawful presence* — o erro mais caro e mais comum). Mapear inadmissibilidade `8 U.S.C. 1182` (INA 212(a)). Só depois reabrir categorias. |
| **Não**, com fatos claros de status mantido | Seguir o protocolo abaixo. |
| **Nunca esteve nos EUA** | Seguir; ainda assim checar deportação de outro país, fraude de visto, crime, se relevarem. |

Por que é a primeira pergunta: é a variável que **mais muda o caso** e a que o cliente **mais esconde** ou minimiza. Diagnosticar “H-1B lindo” em cima de barra de reentrada é produto que queima o cliente.

Inadmissibilidade (mapa de classes): `8 U.S.C. 1182` — https://uscode.house.gov/view.xhtml?req=granuleid:USC-prelim-title8-section1182  
Waivers (visão de ⚖️): skills `waivers-i601` / `inadmissibilidade-212a` — não “resolver” com frase genérica aqui.

---

## Protocolo (ordem fixa)

### 1. Fatos de elegibilidade (não opinião)

Coletar só o que decide classe:

1. **Situação geográfica** — fora dos EUA × dentro em status × dentro fora de status (já no gate zero).
2. **Objetivo** — temporário com retorno × permanente × proteção.
3. **Base familiar** — cidadão/LPR; grau (cônjuge, filho, pai, irmão…).
4. **Base laboral / empresa** — oferta, multinacional, habilidade extraordinária, tratado E.
5. **Estudo / intercâmbio** — programa, funding, laços no exterior.
6. **Histórico de imigração** — vistos negados, 214(b), 221(g), remoção, *misrepresentation*.
7. **Criminalidade / fraude / saúde** — se houver indício, flag 212(a) **sem** inventar resultado.

### 2. Bifurcação imigrante × não-imigrante

Rodar a lógica de `imigrante-x-nao-imigrante`:

- Não-imigrante = classes `8 U.S.C. 1101(a)(15)` — https://uscode.house.gov/view.xhtml?req=granuleid:USC-prelim-title8-section1101  
- Presunção de imigrante em muitas classes: **INA 214(b)** / `8 U.S.C. 1184(b)` — https://uscode.house.gov/view.xhtml?req=granuleid:USC-prelim-title8-section1184  
- Manutenção/extensão: `8 CFR 214` — https://www.ecfr.gov/current/title-8/chapter-I/part-214  
- Mudança de status (quando aplicável): `8 CFR 248` — https://www.ecfr.gov/current/title-8/chapter-I/part-248

### 3. Matriz: alcança / fechada / condicional

Para **cada** categoria candidata, classificar:

| Selo | Significa |
|---|---|
| ✅ **Alcançável em tese** | Base fática + classe estatutária existem; ainda falta dossiê e adjudicação |
| 🟡 **Condicional** | Falta fato, dual-intent tensionado, fila, waiver, dual representation, vigência (TPS) |
| 🔴 **Fechada neste caso** | Sem base legal, barra, status proíbe, categoria não dual-intent com plano de imigrar agora, etc. |

**Nunca** transformar 🟡 em ✅ por marketing. **Nunca** esconder 🔴.

### 4. Filtros que fecham rota (sem número de cota/fila)

| Filtro | Efeito típico |
|---|---|
| Sem laços / intenção permanente em B/F típico | 214(b) — rota turística/estudo **fechada** como “morar” |
| Fora de status + saída planejada | Risco de barras 3/10 — ver `barras-3-10-anos` |
| Sem *qualifying relative* / sem oferta / sem investimento enquadrado | IR/F/EB correspondente **fechado** |
| TPS “do país X” de memória | ⛔ Checar country page no dia (`varredura-de-vigencia`) |
| DACA **inicial** | Acionar `varredura-de-vigencia`, abrir https://www.uscis.gov/DACA no dia e devolver URL + data; enquanto o estado de referência persistir, dizer “aceita, mas não processada” — **nunca** “obtenível” (TRAVA 7) |
| Matéria inland + só OAB | Representação perante DHS inland **não** é do advogado BR — `trava-de-representacao` |

Preferências e cotas familiares/emprego: estatuto `8 U.S.C. 1151`–`1153` — https://uscode.house.gov/ (sem cut-off hardcoded; Visa Bulletin só URL no dia: https://travel.state.gov ).  
Ajuste de status (visão): `8 U.S.C. 1255` — https://uscode.house.gov/view.xhtml?req=granuleid:USC-prelim-title8-section1255 · regulamento parte 245 no eCFR.

### 5. Ônus da prova

`8 U.S.C. 1361` (INA 291): em geral, o ônus de provar elegibilidade é do requerente.  
https://uscode.house.gov/view.xhtml?req=granuleid:USC-prelim-title8-section1361  

Desde **PA-2026-05**, falta de *initial evidence* pode gerar **negativa sem RFE/NOID**. Diagnóstico “elegível em tese” **não** dispensa `dossie-pre-protocolo`.  
PDF: https://www.uscis.gov/sites/default/files/document/policy-manual-updates/20260805-EvidentiaryStandards.pdf

---

## Formato de saída (obrigatório)

```text
## Diagnóstico de elegibilidade
- Data: AAAA-MM-DD
- Gate zero (fora de status / UP): SIM | NÃO | INCERTO → barras-3-10-anos? SIM/NÃO
- Objetivo: temporário | permanente | proteção
- Situação: fora EUA | EUA em status | EUA fora de status

### Alcançáveis em tese (✅)
- [categoria] — base fática: … — dispositivo: … — URL: …

### Condicionais (🟡)
- [categoria] — o que falta / risco: … — skill de aprofundamento: …

### Fechadas neste caso (🔴)
- [categoria] — motivo normativo ou fático: …

### Próximos passos
- mapa-de-caminhos | skill C3/C4/C5 | dossie-pre-protocolo | waivers | attorney EUA
- Disclaimer: sem garantia de aprovação; adjudicação caso a caso.
```

---

## Por frente

| Frente | Tom do diagnóstico |
|---|---|
| 👤 | Linguagem clara; o que **pode** e o que **não** pode; por que a barra ou o 214(b) trava |
| ⚖️ | Dispositivo + URL; flags de inadmissibilidade; se inland, quem representa (292.1) |
| 💼 (consumo) | Só categorias honestas; se 🔴, **não vender**; ver `o-que-nao-vender` / *Avoid Scams* https://www.uscis.gov/avoid-scams |

## O que esta skill **não** faz

- Não calcula dias de *unlawful presence* (só aponta a skill).
- Não preenche formulário nem promete aprovação.
- Não hardcoda taxa, cota, cut-off ou processing time.
- Não trata Policy Manual como direito acionável (TRAVA 8).

## Encadeamento

`triagem-por-conversa` → **esta** → `mapa-de-caminhos` e/ou `linha-do-tempo-do-caso` → skill de categoria → `dossie-pre-protocolo`.

## Guard

1. **Pergunta de fora de status / UP antes de qualquer recomendação.**  
2. Apontar `barras-3-10-anos` quando SIM/INCERTO.  
3. Separar ✅ / 🟡 / 🔴 com honestidade.  
4. Toda afirmação normativa: dispositivo + URL oficial.  
5. Zero número operacional no corpo — só URL.  
6. Não reescrever os gates C1; citá-los.
