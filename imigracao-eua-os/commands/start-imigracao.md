---
description: Onboarding do plugin imigracao-eua-os. Por botões: frente (imigrante/comercial/advogado), destino (EUA nesta versão), situação atual e urgência. Use na primeira abertura ou para reconfigurar.
---

# /start-imigracao

Configuração inicial do plugin **imigracao-eua-os**.

Aciona a skill **`onboarding-imigracao`**, que pergunta com botões (AskUserQuestion) nas listas fechadas:

1. **Frente** — 👤 imigrante · 💼 comercial · ⚖️ advogado
2. **Destino** — EUA (único completo em v0.1); outros países da família ficam fora de escopo nesta versão
3. **Situação atual** — no Brasil / nos EUA em status / nos EUA fora de status / não sei
4. **Urgência** — pensando · montando dossiê · protocolado · deu problema

⛔ Se a situação for **nos EUA fora de status**, a skill **não minimiza** — aponta `barras-3-10-anos` como leitura obrigatória antes de qualquer rota.

Depois do onboarding, devolve o operador ao `imigracao-master` / `/imigracao`.
