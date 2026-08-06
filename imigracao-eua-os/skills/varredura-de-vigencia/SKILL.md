---
name: varredura-de-vigencia
description: "GATE 1 anti-defasagem. Antes de qualquer resposta operacional que toque litígio H.R.1/Pub.L.119-21, TPS, Visa Bulletin ou taxas, lê a fonte oficial no dia e devolve a data da consulta. Quatro camadas se movem sozinhas por ato do executivo ou da corte — não por lei lenta. Use quando for afirmar estado de pagamento vacatado, país em TPS, cut-off de fila, fee schedule, processing time, policy alert recente, ou qualquer fato que o treino do modelo possa ter congelado. Nunca responde de memória se a fonte do dia não foi lida."
---

# VARREDURA-DE-VIGÊNCIA ⭐ GATE 1 — anti-defasagem

> **Camada C1 · Fundação.** Frentes: 👤 imigrante · 💼 comercial · ⚖️ advogado.
> Roda **antes** de qualquer skill operacional afirmar estado de fato móvel.
> Análogo do `varredura-jurisprudencial-pre-tese` do bancário: aqui o risco não é tese vencida — é **lei/política que mudou por ato do executivo (ou liminar) na semana passada**, e o modelo responde desatualizado **com confiança**.

## Quando ativar (obrigatório)

Antes de afirmar qualquer item destas **quatro camadas móveis**. Se a resposta tocar uma delas e a fonte do dia **não** foi lida → **não afirmar**; declarar a lacuna.

| # | Camada | O que muda sozinho | Onde ler **no dia** |
|---|---|---|---|
| 1 | Litígio da H.R. 1 / Pub. L. 119-21 | vacatur, stay, apelação, intenção do DHS de cobrar | https://www.uscis.gov/newsroom/alerts |
| 2 | Terminações / designações de TPS | *designado* ≠ *vigente*; litígio de terminação por país | country page do país em https://www.uscis.gov (buscar "TPS [país]") |
| 3 | Visa Bulletin | cut-offs e datas de *final action* / *filing* mudam por mês, por desenho | https://travel.state.gov (Visa Bulletin do mês corrente) |
| 4 | Taxas (fee schedule) | G-1055 e fees da Pub. L. 119-21 ajustam; páginas de form podem exibir trechos defasados | https://www.uscis.gov/g-1055 |

Fontes de topo **e só elas** para esta varredura: `uscis.gov` · `travel.state.gov` · `ecfr.gov` · `federalregister.gov` · `dhs.gov` · `uscode.house.gov` · `justice.gov/eoir` · `govinfo.gov`. Blog, escritório e agregador **não** contam como fonte.

## Por que existe (as travas que esta skill materializa)

- **TRAVA 3** do corpus: taxa, cota e cut-off **nunca** hardcoded no corpo de skill — só URL + leitura no dia.
- **TRAVA 4**: a camada H.R. 1 está em **três** casos distintos (não um). Liminar muda de estado. Afirmar "em vigor" **ou** "morto" sem reler o alerta do dia é erro.
- **TRAVA 7**: "designado" ≠ "vigente" em TPS/humanitário. A skill checa a *country page* no dia — nunca de memória.
- **TRAVA 8**: o site do USCIS **não é a lei**; a varredura captura o **estado de política/alerta** e a data, e a cascata de autoridade fica com `mapa-normativo-eua`.

## Protocolo (ordem fixa)

1. **Identificar** quais das 4 camadas a resposta toca (pode ser mais de uma).
2. **Abrir a URL oficial** da tabela (WebFetch / ferramenta de leitura). Não usar cache de sessão antiga se o usuário pedir estado atual.
3. **Registrar na saída**:
   - URL consultada;
   - **data da consulta** (dia civil da leitura);
   - trecho ou título do alerta/página que sustenta a afirmação;
   - se a página não carregou ou ficou bloqueada → **declarar falha de leitura**.
4. **Só então** afirmar o estado. Se não leu → **não afirma de memória**. Diz: *"não pude confirmar na fonte oficial nesta data; o estado depende de [URL]; releia antes de protocolar/orçar."*
5. Se a camada for **H.R. 1**, **não misturar os três litígios** (ver seção abaixo). Nomear o caso e o objeto.

## Camada 1 — H.R. 1 / Pub. L. 119-21 (três casos, não um)

A consolidação do corpus (consulta de referência no alerta USCIS) separa:

| Objeto típico | O que a skill **não** faz |
|---|---|
| Vacatur de guidance de pagamento em certos H-1B | Não funde com stay de outras policies |
| Vacatur de Policy Manual / Policy Alerts específicos | Não generaliza "toda a H.R. 1 caiu" |
| Stay parcial de policies baseadas na H.R. 1 | Não trata stay parcial como morte total da lei |

Regra de saída: liminar **muda de estado**. Toda skill que toque pagamento/requisito da H.R. 1 **relê** https://www.uscis.gov/newsroom/alerts **no dia** e devolve a data. O DHS pode declarar intenção de cobrar se a ordem for derrubada — isso **não** autoriza afirmar vigência plena sem o alerta atual.

## Camada 2 — TPS e humanitário móvel

- Páginas de TPS listam países; **terminação** e **litígio de terminação** alteram o que o cliente pode renovar ou estender.
- ⛔ Proibido: "Haiti/Síria/Iêmen ainda têm TPS" (ou o inverso) **de memória**.
- ✅ Obrigatório: abrir a *country page* do país e citar o status **com data de consulta**.
- Mesma disciplina para DACA (iniciais vs renovações), USRAP e outros programas cujo hub USCIS avisa suspensão/processamento limitado — sempre a página oficial do programa no dia.

## Camada 3 — Visa Bulletin

- Cut-offs **não** são capturados em skill. A skill manda o link do mês e, se a resposta for estratégica (ajustar vs consular, fila F/EB), **lê o bulletin do mês corrente**.
- Se `travel.state.gov` bloquear a leitura automatizada → declarar o bloqueio; **não inventar** *final action date*.

## Camada 4 — Taxas (G-1055)

- Fonte canônica do fee schedule: https://www.uscis.gov/g-1055
- ⛔ Proibido copiar valor em dólar de treino, de página antiga de form, ou de índice de busca.
- ⚠️ Armadilhas vivas do corpus: páginas de form e hubs antigos podem exibir valores pré-reforma. A skill **não** usa o valor da página do form se o G-1055 disser outra coisa — e **não** imprime o número na skill; manda ler o G-1055 no dia.
- Fees da Pub. L. 119-21 / AAF: se o notice individual ou o G-1055 não confirmarem, **não inventar**.

## Formato de saída obrigatório

Toda resposta operacional que passou por este gate inclui um bloco legível:

```text
## Varredura de vigência
- Data da consulta: AAAA-MM-DD
- Camadas tocadas: [1 H.R.1 | 2 TPS | 3 VB | 4 taxas]
- Fontes lidas:
  - <URL> — <título ou achado em 1 linha>
- Resultado: CONFIRMADO | PARCIAL | FALHA DE LEITURA
- Se FALHA/PARCIAL: o que NÃO pode ser afirmado até releitura
```

## O que esta skill **não** faz

- Não substitui `trava-de-representacao` (GATE 2).
- Não cria direito: Policy Alert e página de notícias **não** são o estatuto (`mapa-normativo-eua`).
- Não promete prazo de processamento (mesmo lendo a página de *processing times* — se citar, só com URL + data, nunca como garantia).
- Não inventa resultado de litígio "provável".

## Encadeamento

- **Antes:** `imigracao-master` / triagem identifica o tema.
- **Junto:** se a frente for 💼 ou ⚖️, em seguida `trava-de-representacao`.
- **Depois:** skills de categoria (H, TPS, green card, asilo…) só afirmam o que este gate liberou.

## Guard (inviolável)

1. **Sem fonte do dia + data de consulta = sem afirmação operacional** sobre as 4 camadas.
2. **Zero número de taxa, cota ou cut-off** no corpo desta skill e nas saídas geradas a partir de memória — só URL + o que a página do dia mostrar (e a data).
3. **Não misturar** os três litígios da H.R. 1.
4. **Não** dizer "segundo o site do USCIS" como se fosse a lei — dizer "alerta/página USCIS de [data], sujeito a [estatuto/regra]".
5. Default no incerto: **declarar gap** e mandar reler a URL — nunca completar com o treino do modelo.
