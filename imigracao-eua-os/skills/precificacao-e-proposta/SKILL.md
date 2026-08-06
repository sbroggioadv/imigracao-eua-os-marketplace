---
name: precificacao-e-proposta
description: "Monta proposta comercial de imigração BR→EUA com TRÊS linhas separadas: honorário do operador Brasil (A) × taxas de governo (só URL G-1055 lida no dia, zero valor hardcoded) × honorário do correspondente attorney EUA (B). Espelha a linha geográfica e a arquitetura A/B/C. Use ao orçar, enviar proposta, revisar tabela de preços ou embutir fee de governo no pacote. Nunca imprime dólar de taxa federal no corpo da skill nem na proposta gerada a partir de memória."
---

# PRECIFICAÇÃO-E-PROPOSTA — três linhas, zero taxa inventada

> **Camada C7 · Frente comercial.** Frentes: **💼 comercial**.  
> Gates: `trava-de-representacao` (sempre) · `varredura-de-vigencia` **obrigatória** na linha de taxas · `arquitetura-do-servico` para saber o que se cobra.  
> Fee schedule oficial: https://www.uscis.gov/g-1055  
> Avoid Scams: https://www.uscis.gov/avoid-scams  
> eCFR 292.1: https://www.ecfr.gov/current/title-8/chapter-I/part-292/section-292.1

## Linha geográfica (na proposta, em uma frase)

Quem cobra **representação federal inland** é o *attorney* da camada B (G-28).  
O prestador só-OAB cobra camada A (direito BR / educação / dossiê / referral) e, **só se encaixar**, representação sob `292.1(a)(6)` fora dos EUA — discricionária (`faixa-292-1-a-6`).

---

## 1. As três linhas (estrutura inviolável)

Toda proposta comercial **discrimina** no mínimo:

| Linha | O que é | Quem recebe | Como precificar |
|---|---|---|---|
| **1 — Honorário A (Brasil)** | Direito BR, educação geral, dossiê, coordenação, referral; opcional (a)(6) se aplicável | Operador BR | Livre negocial + ética OAB; **escopo escrito** (`contrato-e-escopo`) |
| **2 — Taxas de governo** | Filing fees, biometrics e demais custas oficiais do benefit request / visto | Tesouro / agência (USCIS, DOS, etc.) — **não** é lucro de A | **Só** ler a fonte no dia — ⛔ **nenhum valor em dólar** no texto da skill nem copiado de memória |
| **3 — Honorário B (correspondente EUA)** | *Practice* / aparência G-28, estratégia federal inland, resposta a RFE com tese, etc. | Attorney (ou estrutura autorizada) nos EUA | Acordo B–C ou A–B transparente; **não** misturar com linha 1 sem discriminação |

Opcional (quarta linha de **custos de terceiros**, se houver): cartório BR, apostila, tradução, correios, exames — sempre discriminados, sem chamar de “taxa USCIS”.

---

## 2. Linha 2 — taxas de governo (TRAVA 3)

### Obrigatório na proposta

```text
TAXAS DE GOVERNO (estimativa sujeita a confirmação)
- Fonte canônica USCIS (fee schedule): https://www.uscis.gov/g-1055
- Data em que o orçamento leu o G-1055: AAAA-MM-DD
- Formulários previstos neste caso: [lista de form numbers]
- Observação: fees da legislação recente podem ser non-waivable ou ajustar
  periodicamente — releia o G-1055 e a página do form no dia do pagamento.
- Taxas consulares / DOS (se houver): ler a página oficial do Department of State
  no dia (travel.state.gov) — não usar valor de blog.
```

### ⛔ Proibido

1. Colocar no corpo da skill ou na proposta gerada **de memória** qualquer quantia em dólar de filing fee, biometrics, AAF, etc.  
2. Usar trechos indexados de páginas de form defasadas (armadilha viva do corpus).  
3. Dizer “taxa inclusa no pacote” **sem** discriminar o que é honorário e o que é governo.  
4. Prometer *fee waiver* ou redução sem base no form/instruções vigentes do dia.

### Protocolo `varredura-de-vigencia` (camada 4 — taxas)

Antes de fechar orçamento que mencione custo oficial:

1. Abrir https://www.uscis.gov/g-1055  
2. Registrar **data da consulta**  
3. Se a página não carregar → **não inventar**; proposta sai com “taxa a confirmar no G-1055”  
4. Só então o humano/agente cola o valor **lido hoje** na proposta do cliente (o valor vive na proposta datada, **não** nesta skill)

---

## 3. Linha 1 — honorário A (como montar)

### Por pacote de escopo (recomendado)

| Pacote | Inclui (exemplos) | Não inclui |
|---|---|---|
| **Educação + mapa** | sessão de orientação, glossário, comparação de rotas **sem** *practice* | G-28, parecer de elegibilidade como attorney US |
| **Ponte Brasil** | certidões, apostila, tradução pública (eixo BR), menor | filing federal |
| **Dossiê pré-protocolo** | checklist, organização de provas, revisão de completude (TRAVA 2) | garantia de aprovação; aparência inland |
| **Coordenação A+B** | briefing ao attorney, tradução de contexto, agenda | honorário de B (linha 3) |
| **Representação (a)(6)** | só se checklist de `faixa-292-1-a-6` fechar; preço **condicionado** à aceitação do oficial | equivalência a bar US |

### Critérios de precificação (sem número mágico)

- Complexidade fática (vínculos, criminal, status irregular → `barras-3-10-anos`).  
- Volume documental e necessidade de ponte BR (C8).  
- Se haverá B (coordenação custa tempo de A).  
- Risco de recusa de aparência (a)(6) — preço de representação federal **não** se vende como certo.  
- Ética: honorário compatível com o que o contrato **pode** entregar (`o-que-nao-vender`).

---

## 4. Linha 3 — honorário do correspondente

- Orçar **depois** de ter B identificado ou faixa de B (`rede-de-correspondentes`).  
- Deixar claro: B define a estratégia federal inland e a aparência; A não “revende bar americana” sem B real.  
- Modelos: (i) cliente paga B direto; (ii) A repassa e discrimina; (iii) B fatura e A fatura só coordenação.  
- Nunca apresentar honorário de B como “taxa USCIS”.

---

## 5. Template de proposta (esqueleto)

```text
PROPOSTA — serviço de apoio a imigração EUA
Data: AAAA-MM-DD
Cliente: …
Locus da matéria (dentro × fora dos EUA): …
Arquitetura: A = … / B = … (ou “pro se + A”) / C = cliente

1. HONORÁRIO — OPERADOR BRASIL (A)
   Escopo: …
   Valor: [moeda local / forma de pagamento]
   Fora do escopo: representação inland; G-28; garantia de resultado

2. TAXAS DE GOVERNO
   Ver https://www.uscis.gov/g-1055 (consulta em AAAA-MM-DD)
   Forms previstos: …
   Valores: [preencher só com leitura do dia — não inventar]

3. HONORÁRIO — ATTORNEY / CORRESPONDENTE EUA (B)
   Escopo: aparência G-28 / practice conforme engagement de B
   Valor: … | ou “sob orçamento de B após aceite”

4. CUSTOS DE TERCEIROS (se houver)
   …

Declarações:
- Não garantimos aprovação nem prazo de processamento
  (https://www.uscis.gov/avoid-scams).
- Modelo = conformidade com 8 CFR 292.1; não somos “autorizados pelo USCIS”
  como consultores federais BR→US.
- Se (a)(6): aparência sujeita a discricionariedade do oficial.
```

---

## 6. Erros que matam a proposta (checklist)

| Erro | Correção |
|---|---|
| Um preço único “pacote green card all-in” sem discriminação | Separar linhas 1–2–3 |
| “Taxa de governo = US$ X” copiada de chat antigo | G-1055 no dia + data |
| “Inclui advogado nos EUA” sem B nomeado ou processo de escolha | `rede-de-correspondentes` |
| “Garantido em X meses” | Remover — Avoid Scams |
| Só-OAB cobrando “representação no USCIS” inland | Bloquear — linha geográfica |
| (a)(6) cobrado como se fosse bar US | Renomear e condicionar |

---

## 7. Encadeamento

`arquitetura-do-servico` → escopo em `contrato-e-escopo` → **esta skill** → se B: `rede-de-correspondentes` → copy em `captacao-honesta` → filtro final `o-que-nao-vender`.  
Se a proposta citar fila/Visa Bulletin/litígio H.R.1: GATE 1 (`varredura-de-vigencia`) — **sem** cut-off hardcoded.

## Guard

1. **Três linhas** sempre discriminadas.  
2. ⛔ **Nenhum valor** de taxa de governo no texto desta skill.  
3. Proposta datada + URL G-1055 + data de leitura.  
4. Linha geográfica e A/B/C explícitos.  
5. Sem promessa de prazo/resultado.  
6. (a)(6) só com discricionariedade no preço e no texto.
