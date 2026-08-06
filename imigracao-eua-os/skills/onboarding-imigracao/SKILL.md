---
name: onboarding-imigracao
description: "Primeira conversa do imigracao-eua-os. Por botões (AskUserQuestion): frente (imigrante/comercial/advogado), país de destino (fixo EUA nesta versão), situação atual (Brasil / EUA em status / EUA fora de status) e prazo. Grava o perfil. Se estiver nos EUA fora de status, não minimiza — aponta barras-3-10-anos como leitura obrigatória. Use na primeira abertura, /start-imigracao, configurar, quero começar."
---

> **🖱️ Escolhas = botões:** nas perguntas de **lista fechada** use **AskUserQuestion** (máx. 4 opções; se houver mais, divida). Não peça para digitar 1/2/3.

# ONBOARDING-IMIGRACAO — `/start-imigracao`

> Camada 0 · frentes **👤 💼 ⚖️**. Porta de entrada, roda **uma vez** (ou ao reconfigurar). Fixa quem opera e o estado do caso — **sem** produzir peça nem prometer resultado.

## Anexos obrigatórios (`context/`)
- `anexo-trava-representacao.md` — lembrar a linha geográfica cedo (quem pode representar).
- `anexo-policy-alerts-2026.md` — PA-2026-05 (dossiê completo) e PA-2026-04 (attorneys).

## Objetivo e quando ativar
Gravar **frente · destino · situação · urgência** e devolver o operador ao `imigracao-master`. Roda na **primeira** sessão (sem perfil) ou quando pedirem reconfigurar.

## Disclaimer (dizer na entrada, uma linha)
Este plugin **não substitui** advogado licenciado nos EUA quando a matéria é dentro do território americano. É ferramenta de diagnóstico, dossiê e compliance — não garantia de visto ou green card.

## Pergunta 1 (botões) — FRENTE
- 👤 **Imigrante** — quero ir / entender caminhos / checklist.
- 💼 **Comercial** — monto ou vendo o serviço (proposta, contrato, rede).
- ⚖️ **Advogado** — monto a peça / o dossiê / o recurso.
- **Só estudar o plugin** — mapa das camadas, sem caso ativo.

## Pergunta 2 (botões) — PAÍS DE DESTINO
- **Estados Unidos** — único país **completo** nesta versão (v0.1).
- **Outro (PT / ES / PY / UY…)** — dizer com honestidade: família de imigração **prevista**, ainda **não** neste plugin; não improvisar norma estrangeira.
- **Ainda não sei** — manter EUA como default de estudo e avisar a limitação.
- **Mais de um país** — gravar EUA como foco desta sessão; outros ficam fora de escopo.

## Pergunta 3 (botões) — SITUAÇÃO ATUAL
- **No Brasil (ou fora dos EUA)** — via consular / não-imigrante / imigrante a partir do exterior.
- **Nos EUA em status** — status válido; cuidado com *unlawful presence* futura e com *overstay*.
- **Nos EUA fora de status** — ⛔ **não minimizar** (ver bloco abaixo).
- **Não sei classificar** — não chutar; pedir fatos (entrada, visto, I-94, pendências) via `triagem-por-conversa` depois do onboarding.

### ⛔ Se a resposta for “nos EUA fora de status”
1. **Não** dizer “é só regularizar”, “fica tranquilo” nem “entra com ajuste depois”.
2. Apontar como **leitura obrigatória** a skill `barras-3-10-anos` (*unlawful presence* — o erro mais caro e mais comum do corpus).
3. Avisar que barras e inadmissibilidade (INA 212(a) / 8 U.S.C. 1182) dependem de fatos e de **representação autorizada** se houver procedimento dentro dos EUA.
4. Âncora de mapa de inadmissibilidade (estatuto): `https://uscode.house.gov/` (título 8) e regulação em `https://www.ecfr.gov/current/title-8` — **sem** diagnosticar a barra no onboarding.
5. Handoff: `imigracao-master` → GATE 1 `varredura-de-vigencia` → `barras-3-10-anos` **antes** de qualquer mapa de caminhos otimista.

## Pergunta 4 (botões) — PRAZO / URGÊNCIA (subjetivo do usuário)
- **Sem pressa** — exploração e mapa de caminhos.
- **Tenho um marco pessoal** (estudo, trabalho, família) — triagem + elegibilidade.
- **Já tem protocolo / prazo de governo correndo** — ⛔ não inventar dias; ler o **notice** e a fonte no dia; se RFE/NOID, ir a `resposta-a-rfe-noid` (prazo é o do aviso; correio = regra de 8 CFR 103.8(b), **não** a prática antiga de acréscimo internacional extra).
- **Situação de risco** (detenção, NTA, remoção) — ⚖️ + representação autorizada; `removal-eoir-bia-aao` só com quem pode representar (292.1).

> Esta pergunta mede **urgência subjetiva**, não autoriza escrever prazo de processamento do USCIS/DOS como número.

## O que dizer na entrada — sem promessa (as travas em linguagem curta)
1. **Quem representa:** lista fechada do 8 CFR 292.1; linha **geográfica** — dentro dos EUA o advogado só OAB **não** representa; fora, (a)(6) discricionário. Fonte: `https://www.ecfr.gov/current/title-8/chapter-I/subchapter-B/part-292`.
2. **Dossiê completo:** desde o PA-2026-05 o USCIS pode **negar sem RFE e sem NOID** se faltar initial evidence. Espinha = `dossie-pre-protocolo`. PDF: `https://www.uscis.gov/sites/default/files/document/policy-manual-updates/20260805-EvidentiaryStandards.pdf`.
3. **Números oficiais mudam:** taxa, cota, Visa Bulletin e processing time **não** vêm da memória do plugin — vêm da URL no dia.
4. **Sem garantia de resultado ou de prazo** — critério *Avoid Scams*: `https://www.uscis.gov/avoid-scams`.
5. **Policy Manual não é lei** — cascata: estatuto → regulamento → PM → alerta.
6. 🔒 **Despersonalização:** grave função, frente e situação — **nunca** nome civil de cliente, A-Number, passaporte, e-mail pessoal ou número de processo em artefato compartilhado.

## O que este onboarding **não** faz
- Não escolhe a categoria de visto sozinho (isso é `diagnostico-de-elegibilidade` / `mapa-de-caminhos`).
- Não redige petição, G-28, G-28I nem DS-160.
- Não calcula *unlawful presence* em dias (só aponta a skill e o risco).
- Não dá preço de honorários nem de taxa governamental.

## Entrega obrigatória final
3–6 linhas gravadas no perfil da sessão:
- **Frente** (👤/💼/⚖️/estudo)
- **Destino** (EUA nesta versão)
- **Situação** (BR · EUA em status · EUA fora de status · indefinida)
- **Urgência** (exploração · marco pessoal · prazo de governo · risco)
- Se **fora de status**: flag `LEITURA_OBRIGATORIA=barras-3-10-anos`
- Handoff explícito ao `imigracao-master` (que abrirá GATE 1 e, se 💼/⚖️, GATE 2)

## Guard
Não produzir peça nem parecer aqui. Não minimizar *unlawful presence*. Não prometer regularização fácil, prazo de aprovação nem “sempre cabe ajuste”. Se destino ≠ EUA, **dizer** o limite da versão. Se situação = fora de status, **bloquear** mapa de caminhos otimista até `barras-3-10-anos`.
