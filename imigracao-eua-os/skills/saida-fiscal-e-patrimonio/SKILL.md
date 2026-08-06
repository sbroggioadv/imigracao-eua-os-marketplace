---
name: saida-fiscal-e-patrimonio
description: "Saída fiscal e patrimônio que fica no Brasil quando o cliente emigra. Caminho RFB: comunicação de saída definitiva + Declaração de Saída Definitiva do País (DSDP) + comunicação a fontes pagadoras (IN RFB 208/2002 e correlatas). Zero valor e zero alíquota no corpo — só o caminho e a URL da Receita. Fora de escopo declarado: bitributação BR-EUA, FATCA/FBAR, exit tax americano (lacunas do corpus). Frentes 👤💼⚖️."
---

# SAÍDA-FISCAL-E-PATRIMÔNIO — DSDP · comunicação · o que fica no BR

> **Camada C8 · Ponte Brasil.** Frentes: 👤 imigrante · 💼 comercial · ⚖️ advogado (tributário/civil BR).  
> ⛔ **Nenhum valor, nenhuma alíquota** nesta skill — só o **caminho** e a **URL** oficial.  
> ⛔ **Fora de escopo (lacuna assumida do corpus):** bitributação BR–EUA, FATCA/FBAR, *exit tax* / *covered expatriate* IRS. Remeter a **especialista** (tributarista internacional / counsel US tax).

## O que o cliente precisa entender (👤)

- Ter *green card*, visto longo ou morar fora **não** "fecha" automaticamente o IRPF brasileiro.  
- **Saída fiscal** (comunicação + DSDP) é regime da **Receita Federal do Brasil**.  
- O MRE registra que a saída definitiva **produz efeitos fiscais** e **não** impede, por si, o acesso a serviços consulares — ler a página MRE no dia:  
  https://www.gov.br/mre/pt-br/assuntos/portal-consular/saida-fiscal-definitiva-do-brasil  

---

## Caminho oficial (RFB) — sem números

Fontes a **abrir no dia** (não cachear prazo/valor):

| Passo | O quê | URL |
|---|---|---|
| 1 | **Comunicar** a saída definitiva do país | https://www.gov.br/pt-br/servicos/comunicar-saida-definitiva-do-pais |
| 2 | **DSDP** — Declaração de Saída Definitiva do País (DIRPF em razão da saída / condição de não residente) | https://www.gov.br/receitafederal/pt-br/assuntos/meu-imposto-de-renda/preenchimento/dsdp |
| 3 | **Pagar** o IR apurado **conforme** as regras e o sistema do dia (⛔ sem alíquota aqui) | orientações na página DSDP / e-CAC |
| 4 | **Avisar fontes pagadoras** para retenção correta na condição de não residente | serviço gov.br + IN aplicável |

Legislação de referência citada nos serviços RFB: **IN RFB nº 208/2002** e correlatas de DIRPF — buscar o texto atualizado em:

- https://www.gov.br/receitafederal  
- normas oficiais da RFB (portal de legislação da Receita)

Definição operacional (RFB, página DSDP — reler no dia): a DSDP é a declaração de imposto de renda de quem deixa o país com **ânimo definitivo** (não pretende voltar a residir no Brasil) ou se enquadra como **não residente**.

---

## Patrimônio que **fica** no Brasil

A skill **mapeia temas** e **encaminha** — não liquida tributo:

| Tema | O que fazer |
|---|---|
| Imóveis, aluguéis, venda | Renda de fonte BR na não residência; retenção; escritura — tributarista BR |
| Participações societárias / holding | Reorganização, ITCMD, ITBI se integralização — skills da família holding/imobiliário/tributário **BR**, não imigração US |
| Contas, aplicações, previdência | Comunicação a instituições; condição de não residente |
| Procurações / administração | Cadeia cartorária (`cadeia-documental-br` · `apostila-de-haia` se for usar no exterior) |
| Sucessão | Planejamento sucessório BR **≠** *estate tax* US (fora de escopo desta skill) |

⛔ Não misturar "emigrou" com "já resolveu inventário/ITCMD". São frentes distintas.

---

## Protocolo

1. **Ânimo / fato gerador:** saída definitiva vs ausência temporária — a classificação fiscal é da RFB; a skill **não** rotula o cliente sem os critérios oficiais da página do dia.  
2. Abrir as URLs RFB/gov.br acima e registrar **data da consulta**.  
3. Checklist de atos: comunicação → DSDP → fontes pagadoras → (se houver) regularização de pendências no e-CAC.  
4. Separar **fiscal BR** de **imigração US** (duas linhas no contrato comercial).  
5. Se aparecer bitributação, FATCA, FBAR, *exit tax* US → **declarar fora de escopo** e referir especialista.  
6. Zero inventar multa, alíquota, prazo em dias ou valor de DARF.

### Formato de saída

```text
## Saída fiscal e patrimônio (BR)
- Data da consulta RFB: AAAA-MM-DD
- URLs lidas:
  - comunicação: …
  - DSDP: …
- Passos aplicáveis: [ ] comunicar [ ] DSDP [ ] fontes pagadoras
- Patrimônio que permanece no BR: (lista factual do cliente — sem valor de tributo)
- ⛔ Fora de escopo: bitributação · FATCA/FBAR · exit tax US
- ⛔ Nenhum valor/alíquota nesta saída
- Encaminhamento: tributarista BR | counsel US tax (se o cliente insistir no gap)
```

---

## As 3 frentes

| Frente | Entrega |
|---|---|
| 👤 | Entende o **caminho** e as URLs; sabe que visto/green card **não** substitui a RFB |
| 💼 | SKU legítimo: **pacote de saída fiscal BR** (comunicação + DSDP + orientação a fontes) — precifica o **serviço**, não o imposto |
| ⚖️ | Executa/acompanha DSDP e comunicações; coordena patrimônio (holding, ITCMD, ITBI) **sem** se passar por *immigration counsel* nem por tax counsel US nos gaps |

---

## Fora de escopo (obrigatório declarar)

Conforme **ACHADOS-CORPUS** (gap 13) e a régua do plugin:

1. **Tratado / bitributação** Brasil–EUA  
2. **FATCA / FBAR** e obrigações de *U.S. person*  
3. ***Exit tax*** e regras de *covered expatriate* (IRS)  
4. Planejamento de *estate tax* americano  

Esses temas **não** são preenchidos com treino do modelo. A skill **nomeia a lacuna** e para.

---

## Guard (inviolável)

1. **Zero** valor em R$ ou US$, **zero** alíquota, **zero** multa numérica.  
2. Só **caminho + URL RFB/gov.br** (+ data).  
3. Marcar bitributação / FATCA / exit tax US como **fora de escopo**.  
4. Não confundir saída fiscal BR com abandono de residência imigratória US.  
5. Entrega 💼/⚖️ de imigração US continua sob `trava-de-representacao`.  
6. IN 208/2002 e correlatas: citar e mandar ler o texto oficial atualizado — não parafrasear artigo de alíquota.
