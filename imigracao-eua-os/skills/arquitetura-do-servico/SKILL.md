---
name: arquitetura-do-servico
description: "Arquitetura A/B/C do serviço de imigração BR→EUA: A = operador Brasil (direito BR, educação geral, dossiê documental, sem G-28 e sem practice de imigração US inland); B = attorney americano que assina G-28 e responde disciplinarmente; C = cliente. Modelo = compliance dentro do 8 CFR 292.1, não status federal. Use ao desenhar oferta, proposta, onboarding comercial, divisão de papéis ou antes de precificar. Cita GATE 2 (trava-de-representacao); não reescreve a lista fechada."
---

# ARQUITETURA-DO-SERVIÇO — camadas A / B / C

> **Camada C7 · Frente comercial ⭐ fosso.** Frentes: **💼 comercial**.  
> Gate obrigatório antes de qualquer entrega desta skill: `trava-de-representacao` (GATE 2) e, se a proposta tocar taxa/fila/litígio, `varredura-de-vigencia` (GATE 1).  
> Anexos: `context/anexo-trava-representacao.md` · PA-2026-04 em `context/anexo-policy-alerts-2026.md`.  
> eCFR Part 292: https://www.ecfr.gov/current/title-8/chapter-I/part-292  
> Policy Alert attorneys: https://www.uscis.gov/sites/default/files/document/policy-manual-updates/20260713-AttorneysAndRepresentatives.pdf

## Linha geográfica (repetir em toda saída comercial)

| Matéria perante o DHS | Só-OAB (sem bar dos EUA) | Quem aparece |
|---|---|---|
| **Dentro** dos confins geográficos dos EUA (INA 101(a)(38)) | Só-OAB **não** representa por essa credencial. Lista fechada: 292.1(a)(1)–(5) | Default comercial = camada **B** (attorney/accredited + G-28); hipóteses (a)(2)/(3)/(5) existem sob requisitos próprios; cliente também pode *pro se* |
| **Fora** dos confins | **Pode** sob `292.1(a)(6)` + G-28I, **a critério do oficial** | Camada A **em nome próprio** só nessa faixa — ver `faixa-292-1-a-6` |

Lista fechada — `8 CFR 292.1(e)`: *except as set forth in this section, no other person… shall represent others*.  
Fonte: https://www.ecfr.gov/current/title-8/chapter-I/part-292/section-292.1

⛔ **Não** chame este desenho de “autorizado pelo USCIS” ou de categoria federal. **Não existe** *immigration consultant BR→US* no CFR. O produto vende **arquitetura de conformidade** — ver TRAVA 1 do corpus e `trava-de-representacao`.

---

## 1. As três camadas (mapa mental)

```text
┌─────────────────────────────────────────────────────────┐
│  C — CLIENTE (imigrante / peticionário / patrocinador)  │
│  decide, assina verdade dos fatos, paga taxas oficiais  │
└──────────────────────┬──────────────────────────────────┘
                       │ contrata / autoriza
        ┌──────────────┴──────────────┐
        ▼                             ▼
┌───────────────────┐       ┌────────────────────────────┐
│ A — OPERADOR BR   │       │ B — CORRESPONDENTE EUA     │
│ OAB / escritório  │  ←→   │ attorney 8 CFR 1.2         │
│ direito BR +      │ ref.  │ assina G-28 · practice     │
│ dossiê + educação │       │ disciplinar 292.3          │
│ ⛔ G-28 inland    │       │                            │
└───────────────────┘       └────────────────────────────┘
```

A e B **não** se fundem no marketing. O cliente precisa saber **quem** faz o quê **antes** do pagamento.

---

## 2. Camada A — operador Brasil (o que cobra e o que **não** faz)

### ✅ Cobra e entrega (legítimo sem fingir *attorney* US)

| Bloco | Conteúdo típico | Âncora |
|---|---|---|
| **Direito brasileiro** | certidões, apostila (cadeia CNJ), tradução pública exigida no Brasil, autorização de menor (ECA), comunicação de saída / patrimônio no Brasil | C8 do plugin; órgãos BR |
| **Educação geral** | mapa de categorias, glossário, diferença AOS × consular **sem** parecer de elegibilidade como *practice* | `8 CFR 1.2` — carve-out ≠ conselho |
| **Dossiê documental** | organização de provas, checklist, pasta pré-protocolo **sem** assinar como representante DHS inland | TRAVA 2: dossiê completo antes de protocolar |
| **Referral documentado** | indicação escrita a *attorney* bar dos EUA ou org *recognized* | contrato + `rede-de-correspondentes` |
| **Faixa (a)(6)** | só se a matéria for **fora** dos EUA e o oficial permitir — skill `faixa-292-1-a-6` | `292.1(a)(6)` + G-28I |

Definições de *practice* / *preparation* / carve-out de preencher formulário com remuneração **nominal** e **sem** se apresentar como qualificado: `8 CFR 1.2` — https://www.ecfr.gov/current/title-8/chapter-I/part-1/section-1.2

### ⛔ Camada A **não** faz

1. Aconselhamento jurídico de imigração americana que configure *practice* / *preparation* sob `1.2` **sem** estar na lista do `292.1`.
2. Entrar no **G-28** (aparência de *attorney* / accredited nos EUA) — formulário e regras: https://www.uscis.gov/g-28 · `8 CFR 292.4`.
3. Dizer “protocolamos no USCIS” / “representamos você no field office” em caso **inland** só-OAB.
4. Vender-se como *accredited representative* (exige org nonprofit — ver `o-que-nao-vender`).
5. Prometer prazo de processamento ou resultado de benefício — `https://www.uscis.gov/avoid-scams`.

---

## 3. Camada B — correspondente nos EUA

| Papel | Detalhe |
|---|---|
| Quem é (default comercial B) | *Attorney* no sentido de `8 CFR 1.2` (bar da highest court de Estado/território/DC, *good standing*) **ou** accredited rep de org reconhecida (`8 CFR 1292`). Isso **não** apaga as hipóteses excepcionais 292.1(a)(2) law student/graduate, (a)(3) reputable individual e (a)(5) accredited official, cada qual sob seus requisitos |
| O que assina | Aparência no formulário prescrito (**G-28** em matéria inland / perante USCIS nos EUA) — `8 CFR 292.4` |
| Responsabilidade | Conduta profissional e disciplina — `8 CFR 292.3` + PA-2026-04 (`1 USCIS-PM Part D`) |
| Relação com A | B **não** é “funcionário fantasma” de A. Contrato A–B e A–C deixam claro que a *practice* federal inland é de B |

Como escolher e checar B: skill `rede-de-correspondentes`.

---

## 4. Camada C — cliente

- **Dono dos fatos.** Mentira ou omissão no formulário é do cliente (e pode ser fraude).
- **Assina** autorizações (G-28/G-28I quando houver representante), declarações e prova.
- **Paga taxas de governo** na fonte oficial do dia (A e B **não** “embutem” taxa de governo sem discriminar — ver `precificacao-e-proposta` + https://www.uscis.gov/g-1055).
- Pode optar por *pro se* + apoio A (dossiê/educação/direito BR) **sem** B — aí **ninguém** entra em aparência; A não vira representante por omissão.

---

## 5. Fluxos típicos (escolha guiada)

| Cenário | Arquitetura |
|---|---|
| Cliente no Brasil montando consular / DS-160 / documentos BR | A forte (dossiê + ponte BR); B só se houver *benefit request* DHS com aparência |
| Ajuste de status / field office / matéria **dentro** dos EUA | **B obrigatório** para representação; A = BR + dossiê + coordenação |
| Matéria DHS **fora** dos confins + só-OAB quer aparecer | Avaliar `faixa-292-1-a-6` — discricionário; **não** vender como bar americana |
| Escritório quer “só consultoria de imigração US” sem B | ⛔ Redesenhar ou recusar — ver `o-que-nao-vender` |

---

## 6. Protocolo de saída (toda proposta / pitch)

1. Rodar `trava-de-representacao` (e GATE 1 se houver taxa/fila).
2. Declarar **onde** está a matéria (dentro × fora).
3. Nomear **A / B / C** com verbos concretos (o que cada um entrega).
4. Se inland e só-OAB: **B** na aparência ou *pro se* explícito — nunca G-28 “do escritório BR”.
5. Encaminhar contrato para `contrato-e-escopo` e números de honorário para `precificacao-e-proposta` (**zero** taxa de governo hardcoded).

### Frases de arquitetura

| Evitar | Usar |
|---|---|
| “Somos seu advogado de imigração nos EUA” (só OAB, inland) | “Camada A no Brasil (direito BR + dossiê); camada B é attorney admitido nos EUA para a aparência perante o DHS” |
| “Estrutura autorizada pelo USCIS” | “Estrutura de **conformidade** com a lista fechada do 8 CFR 292.1 — não é licença federal de consultor” |
| “Protocolamos tudo por você” | “Organizamos o dossiê; quem protocola/aparece é o cliente *pro se* ou o attorney da camada B” |

---

## Encadeamento C7

`trava-de-representacao` → **esta skill** → `faixa-292-1-a-6` (se A atuar em nome próprio fora) → `contrato-e-escopo` → `precificacao-e-proposta` → `rede-de-correspondentes` → `captacao-honesta` / `o-que-nao-vender`.

## Guard

1. Camada A **sem** G-28 inland e **sem** *practice* US fora da lista.
2. Camada B = quem carrega a aparência e a disciplina federal quando a matéria exige representante authorized.
3. Modelo = **compliance**, não *status* concedido pelo USCIS.
4. Linha geográfica nas **duas** direções em toda entrega.
5. Zero número de taxa/cota/prazo de processamento no corpo — só URL.
