---
description: Porta única do plugin imigracao-eua-os — demanda de imigração EUA em linguagem natural (3 frentes: imigrante, comercial, advogado). Aciona o orquestrador imigracao-master com gates de vigência e trava de representação.
argument-hint: [descrição da demanda de imigração EUA]
---

Você foi acionado pelo comando `/imigracao` do plugin **imigracao-eua-os**.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** conduzir a demanda de imigração para os Estados Unidos pela porta master.

## PROTOCOLO

1. **Acionar a skill `imigracao-master`** — porta única do plugin.
2. Na 1ª interação, identificar **frente** (👤 imigrante / 💼 comercial / ⚖️ advogado) e **fase** do caso por botões (AskUserQuestion).
3. Abrir sempre pelos dois gates:
   - `varredura-de-vigencia` — antes de qualquer número/estado operacional móvel;
   - `trava-de-representacao` — linha geográfica 8 CFR 292.1 (dentro NÃO / fora SIM sob (a)(6)).
4. Rotear para a skill da camada certa; fechar com `suprema-corte-imigratoria` + `validador-imigratorio` quando houver entrega normativa.
5. Se o perfil ainda não existir, oferecer `/start-imigracao` sem travar demanda urgente.

**Skill a acionar:** `imigracao-master`.

⛔ Este plugin **não substitui** *attorney* licenciado nos EUA quando a matéria é adjudicada **dentro** do território americano.
