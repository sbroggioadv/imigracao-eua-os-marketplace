# imigracao-eua-os

Sistema operacional de imigração para os **Estados Unidos** — três frentes no mesmo produto:

| Frente | Público | Pergunta |
|---|---|---|
| 👤 Imigrante | quem quer ir | o que eu faço e como monto? |
| 💼 Comercial | advogado ou consultor | como vendo e entrego o serviço? |
| ⚖️ Advogado | quem monta a peça | processo administrativo ou judicial conforme a lei |

## Escopo (honesto)

**58 skills · 8 anexos · 4 commands · hook echo-only · v0.1.1**

Cobre o mapa principal do país: não-imigrante (B→TN e afins), green card (família, EB-1…EB-5, DV), humanitário, naturalização, inadmissibilidade, barras 3/10, waivers, removal (com trava de representação), e a ponte Brasil (apostila, tradução, menor).

**Não é “tudo que existe em imigração americana”.** Gaps materiais ficam **declarados** (não inventados), entre eles:

- PERM/DOL (rito e timing) — Gap 7  
- *Credible fear* / expedited removal — Gap 10  
- *Public charge* detalhado 2026 — Gap 8  
- CSPA, UPL estadual, fiscalidade BR–EUA profunda, *Lozada* — Gaps 6/11/13/14  
- Lista E-1/E-2 e fees/Visa Bulletin — **sempre** lidos no dia (URLs oficiais)

## Gates estruturais

1. **`varredura-de-vigencia`** — taxas, cotas, Visa Bulletin, TPS, DACA e alertas móveis só com URL lida no dia.  
2. **`trava-de-representacao`** — `8 CFR 292.1`: dentro dos EUA, só hipóteses (a)(1)–(5); fora, (a)(6) com OAB + discricionariedade do oficial.

## Comandos

| Comando | Função |
|---|---|
| `/imigracao` | Porta única (orquestrador) |
| `/start-imigracao` | Onboarding por botões |
| `/imigracao-master` | Alias de `/imigracao` |
| `/corte-imigratoria` | Auditoria R1–R4 |

## Instalação

Marketplace público:

`https://github.com/sbroggioadv/imigracao-eua-os-marketplace`

Settings → Plugins → Pessoal → “+” → cola a URL → instala `imigracao-eua-os` → `/start-imigracao` → `/imigracao`.

## Código × compra

- **Código no GitHub:** **não é software livre.** O repositório é público para viabilizar a instalação no Cowork/Claude Code; o direito de usar o código é concedido pela compra — ver [`LICENSE`](./LICENSE).
- **Compra Kirvano:** licença de uso do plugin na versão adquirida + manual, capa, onboarding e **90 dias de suporte técnico** (instalação/uso/packaging — **não** é consultoria jurídica do seu caso).

<sub>As cópias obtidas até 11/08/2026 foram distribuídas sob MIT e permanecem sob MIT; nenhuma concessão anterior é revogada.</sub>

## Aviso

Este plugin **não substitui** advogado licenciado nos EUA (*attorney* sob `8 CFR 1.2`) quando a matéria é adjudicada **dentro** do território americano. Não garante aprovação de visto, green card ou naturalização.

## Autoria

IA Combativa · família Adv-OS / OS.
