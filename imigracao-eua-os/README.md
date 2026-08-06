# imigracao-eua-os

Sistema operacional de imigração para os **Estados Unidos** — três frentes no mesmo produto:

| Frente | Público | Pergunta |
|---|---|---|
| 👤 Imigrante | quem quer ir | o que eu faço e como monto? |
| 💼 Comercial | advogado ou consultor | como vendo e entrego o serviço? |
| ⚖️ Advogado | quem monta a peça | processo administrativo ou judicial conforme a lei |

## O que cobre

Catálogo completo do país: não-imigrante (alfabeto B→TN), green card (família, EB-1…EB-5, DV), humanitário, naturalização, inadmissibilidade, barras 3/10 anos, waivers, removal, e a ponte Brasil (apostila, tradução, menor).

**58 skills · 8 anexos de contexto · 4 commands · hook echo-only.**

## Gates estruturais

1. **`varredura-de-vigencia`** — taxas, cotas, Visa Bulletin, TPS, DACA e alertas H.R.1 só com URL lida no dia.
2. **`trava-de-representacao`** — `8 CFR 292.1`: dentro dos EUA, só hipóteses (a)(1)–(5); fora, (a)(6) com OAB + discricionariedade do oficial.

## Comandos

| Comando | Função |
|---|---|
| `/imigracao` | Porta única (orquestrador) |
| `/start-imigracao` | Onboarding por botões |
| `/imigracao-master` | Alias de `/imigracao` |
| `/corte-imigratoria` | Auditoria R1–R4 |

## Instalação (cliente)

Marketplace GitHub público + UI Cowork: Settings → Plugins → Pessoal → “+” → cola a URL do marketplace.

## Autoria

IA Combativa · família Adv-OS / OS.

## Aviso

Este plugin **não substitui** advogado licenciado nos EUA (*attorney* sob `8 CFR 1.2`) quando a matéria é adjudicada **dentro** do território americano. Não garante aprovação de visto, green card ou naturalização.
