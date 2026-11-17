---
tipo: "rubrica"
status: "aprovado"
aprovado_em: 2026-11-17
aprovado_por: "Nathalia Locatelli"
curso: "[[MBA IA Aplicada - Início]]"
sprint: "Sprint 12 - Projeto Final - Caso Aplicado Integrado"
gerado_em: 2026-11-17
---

%% fonte interna: [[Projeto Final - página sem banca (para colar)]] (versão sem banca, colada no Notion em 2026-11-17): "O que você entrega" (cinco peças), "Os três casos" (núcleo mínimo e restrição), "O que não é exigido", "Como você será avaliado" (sete critérios em três níveis), "Entradas da demonstração", "Situações eliminatórias", "Nota e reentrega", "As três perguntas que o dossiê responde", "Antes de enviar" (checklist) e "Formato de entrega". Formato: [[Rubrica do aluno (formato)]]. Sem job, por decisão da autora. %%

# Critérios do tutor · Projeto Final (Caso Aplicado Integrado)

**Escala:** Concluído | Recomendação (parcial) | Não concluído ✅ 🟡 ❌
**Pontuação:** ✅ vale os pontos do critério, 🟡 vale metade e ❌ vale zero.
**Pontuação total:** **100 pts** · **Aprovação:** 60 pts e nenhum eliminatório.

> **Como os três níveis da página viram pontos.** Cada critério da página tem duas linhas. A linha **Base** cobre o nível *Suficiente* e vale cerca de dois terços dos pontos. A linha **Excelência** cobre o que o nível *Excelente* acrescenta. *Insuficiente* é ❌ na Base.
> Um projeto todo no nível Suficiente soma 67 pontos e é aprovado; um projeto todo Excelente soma 100.

## Antes de pontuar
1. **Abra o link numa janela anônima.** Se a pasta não abrir, não corrija: devolva ao aluno pedindo a permissão. Isso não é eliminatório, é entrega não avaliada.
2. **Confira se a pasta `ProjetoFinal_NomeSobrenome` tem tudo:**
   - o dossiê em PDF;
   - o pacote do protótipo (export do fluxo ou prints, instrução de sistema em `.txt`, base de conhecimento e log de execuções);
   - o registro de testes;
   - o one-pager;
   - o vídeo de até 3 minutos.
3. **Confira os eliminatórios.** Se algum for acionado, o projeto é reprovado, seja qual for a pontuação:

| Eliminatório | Como verificar |
| --- | --- |
| Protótipo não verificável | O vídeo mostra execução contínua, sem corte e com horário visível, **ou** você consegue executar o protótipo em até 48 horas após a entrega. Se nenhum dos dois acontecer, aciona. |
| Declaração de uso de IA ausente | A última seção do dossiê diz quais ferramentas de IA foram usadas para produzir o documento, em que etapas e o que foi verificado manualmente. Se a seção não existe, aciona. Se está incompleta, não aciona: vira 🟡 em "Métricas e evidência". |
| Dado real identificável | Nomes, CPFs, carteirinhas ou CNPJs reais de cliente ou paciente no dossiê, no registro, no vídeo ou nos prints. Os dados fictícios do pacote do caso não acionam. |

## Parte 1: Diagnóstico e enquadramento (15 pts)
| Critério | Descrição | ✅Concluído | 🟡Recomendação | ❌Não concluído | Pts |
| --- | --- | --- | --- | --- | --- |
| Base | O problema é descrito com número (bloco 1 do dossiê) | O problema tem pelo menos um número do caso, com origem (ex.: 900 solicitações por mês e 2 dias de primeira resposta, no Caso A) | Tem número, mas sem dizer de onde veio | O problema é descrito só com adjetivos ("lento", "caro") | 10 |
| Excelência | Linha de base e escolha justificada (blocos 1 e 2) | O número tem linha de base, e a oportunidade escolhida é justificada contra pelo menos uma alternativa descartada | Tem linha de base, mas a escolha não é comparada com alternativas (ou o contrário) | Sem linha de base e sem comparação | 5 |

## Parte 2: Desenho da solução (15 pts)
| Critério | Descrição | ✅Concluído | 🟡Recomendação | ❌Não concluído | Pts |
| --- | --- | --- | --- | --- | --- |
| Base | Fluxo com separação de responsabilidades (bloco 3) | O fluxo separa com clareza o que é automação, o que é agente e o que fica com humano | A separação existe, mas uma etapa fica ambígua | O fluxo não separa responsabilidades | 10 |
| Excelência | Separação justificada, com diagrama legível | A separação é justificada por tolerância ao erro e volume, e o diagrama é legível sem o texto | Tem diagrama legível, mas a separação não é justificada (ou o contrário) | Sem diagrama, ou diagrama ilegível | 5 |

## Parte 3: Protótipo funcional (15 pts)
| Critério | Descrição | ✅Concluído | 🟡Recomendação | ❌Não concluído | Pts |
| --- | --- | --- | --- | --- | --- |
| Base | Resolve o núcleo mínimo nas entradas da demonstração (vídeo e pacote) | Acerta pelo menos 2 das 3 entradas sem travar, com a instrução de sistema documentada e disparo manual (formulário ou chat) | Acerta 2 de 3, mas a instrução de sistema não está no pacote | Roda só no caminho ensaiado, trava, ou só dispara por e-mail ou agendamento | 10 |
| Excelência | Acerto total e guardrail rastreável | Acerta 3 de 3, e o guardrail dispara com mensagem rastreável, com a tabela entrada · saída sem · saída com | Acerta 3 de 3, mas o guardrail não aparece disparando (ou falta a tabela) | Sem guardrail ativo, ou o guardrail é só uma frase na instrução de sistema | 5 |

**O que conta como guardrail** (um dos quatro tipos aceitos, que altere a saída de forma observável):
- recusa ou desvio de escopo;
- mascaramento ou remoção de dado sensível antes da ferramenta;
- limiar de confiança que escalona para humano;
- validação determinística fora do modelo, para preço, total e desconto.

**Entrada fora do escopo:** na entrada que o protótipo não resolve, o que pontua é o comportamento.
- Conta como acerto: escalar para humano, declarar baixa confiança ou recusar.
- Conta como erro: inventar uma resposta plausível com número errado.

## Parte 4: Governança e risco (15 pts)
| Critério | Descrição | ✅Concluído | 🟡Recomendação | ❌Não concluído | Pts |
| --- | --- | --- | --- | --- | --- |
| Base | Registro de risco com mitigação (bloco 4) | Nomeia o risco principal do caso e uma mitigação concreta | O risco é do caso, mas a mitigação é vaga | Risco genérico ("a IA pode errar"), sem mitigação | 10 |
| Excelência | Mitigação viável no volume e restrição respeitada | A mitigação cabe no volume do caso, e a restrição aparece no desenho (ver tabela abaixo) | Respeita a restrição, mas a mitigação não sobrevive ao volume (ou o contrário) | A restrição do caso é violada no desenho | 5 |

**A restrição de cada caso:**

| Caso | Restrição | O que conferir no desenho |
| --- | --- | --- |
| A · Clínicas | Nome, carteirinha e CPF não trafegam para a ferramenta nova | O diagrama mostra onde esses campos são separados antes da ferramenta; a resposta só é gerada para a categoria sem dado sensível |
| B · Distribuidora | Orçamento de R$ 500 por mês para ferramentas e uso | A busca de preço e o desconto são calculados em passo determinístico, fora do modelo; a conta de ferramentas e uso cabe em R$ 500 |
| C · Contábil | Erro em classificação fiscal gera multa, e o escritório responde por ela | Existe regra de confiança que roteia para humano antes do lançamento |
| Caso próprio | A restrição declarada na primeira página (teto de orçamento, dado sensível ou custo do erro quantificado) | A mesma lógica dos casos da escola, aplicada à restrição declarada |

## Parte 5: Métricas e evidência (15 pts)
| Critério | Descrição | ✅Concluído | 🟡Recomendação | ❌Não concluído | Pts |
| --- | --- | --- | --- | --- | --- |
| Base | Métrica com linha de base e registro de testes real (bloco 5 e Peça 3) | Métrica de resultado com linha de base, e um registro de testes com execuções reais e pelo menos um erro | Tem o registro, mas a métrica não tem linha de base | Sem linha de base, ou registro com 100% de acerto (conta como registro não feito) | 10 |
| Excelência | Contrapeso de qualidade e erro tratado | Métrica de qualidade como contrapeso, e o erro relatado vem com o que o aluno fez a respeito | Só um dos dois | Nenhum dos dois | 5 |

## Parte 6: Conta de operação (15 pts)
| Critério | Descrição | ✅Concluído | 🟡Recomendação | ❌Não concluído | Pts |
| --- | --- | --- | --- | --- | --- |
| Base | Memória de cálculo (bloco 6 e planilha do caso) | A memória de cálculo usa o volume do caso, o custo unitário e declara as chamadas por execução | Tem memória de cálculo, mas falta uma das premissas | Só o número final, sem premissa | 10 |
| Excelência | Revisão humana e variável que mais pesa | Inclui o custo da revisão humana e identifica a variável que mais move o custo | Só um dos dois | Nenhum dos dois | 5 |

**Avalie a memória de cálculo, não o resultado.** Premissa explícita vale mais do que número bonito. Não compare o total com um valor "certo": os preços variam por plataforma e por data.

## Parte 7: Vídeo e one-pager (10 pts)
| Critério | Descrição | ✅Concluído | 🟡Recomendação | ❌Não concluído | Pts |
| --- | --- | --- | --- | --- | --- |
| Base | Vídeo de demonstração e as três perguntas | O vídeo tem até 3 minutos e demonstra as três entradas (duas do pacote e uma do aluno); o dossiê responde as três perguntas | Demonstra as três entradas, mas o dossiê deixa uma pergunta sem resposta | Passa de 3 minutos ou não demonstra | 7 |
| Excelência | Respostas com número e one-pager autônomo | As três perguntas são respondidas com número (inclusive a de custo), e o one-pager tem o formato problema, decisão, solução e resultado, três números e o link do vídeo, e se entende sem conhecer o caso | O one-pager se sustenta, mas uma resposta fica sem número (ou o contrário) | O one-pager cita o nome do caso da escola ou não se entende fora do curso | 3 |

**As três perguntas:**
1. Quanto custa operar isso no volume real do caso, e como chegou a esse número?
2. O que acontece quando a solução erra, e quem percebe antes do cliente?
3. Por que não resolver com automação simples?

## Guia rápido de avaliação
| Intervalo | Descrição |
| --- | --- |
| **90–100 (Excelente)** | Nível excelente em quase todos os critérios: números com origem e linha de base, guardrail disparando com mensagem rastreável, erro tratado, conta com revisão humana e one-pager que funciona fora do curso |
| **75–89 (Bom)** | Base completa em todos os critérios e excelência em parte deles |
| **60–74 (Aprovado)** | Nível suficiente na maioria dos critérios, sem eliminatório |
| **<60 (Insuficiente)** | Algum critério no nível insuficiente que derruba a base (ex.: problema sem número, registro com 100% de acerto, conta sem premissa) |

## O que não deve ser cobrado
| Item | Por quê |
| --- | --- |
| Integração com sistemas reais, interface própria, infraestrutura em nuvem | A página diz que não é exigido e que gastar horas nisso não aumenta a nota |
| Extração de documento digitalizado (Caso C) | Não é exigida: o núcleo mínimo parte do texto já extraído |
| Tratar todos os cenários do caso | Não é exigido: o escopo é o núcleo mínimo (uma iniciativa, um processo, um protótipo) |
| Dado real | Não é exigido (e dado real identificável é eliminatório) |
| Trabalho em equipe | Não é exigido |
| Acertar a entrada fora do escopo | O que pontua é o comportamento (escalar, declarar baixa confiança, recusar) |
| Total "certo" na conta de operação | O avaliado é a memória de cálculo, não o resultado |
| Extensão exata de cada bloco do dossiê | A página dá a extensão como guia (6 a 8 páginas); um bloco mais curto não tira pontos se o conteúdo do critério está lá |
| Plataforma específica | Qualquer uma das plataformas homologadas vale |

## Nota final e reentrega
- **Dois avaliadores corrigem cada entrega de forma independente.** Um não vê a nota do outro antes de fechar a sua.
- **Aprovação:** 60 pontos e nenhum eliminatório.
- **Reprovação:** há uma reentrega em 15 dias, com nota máxima de 70.

## Decisões
- 2026-11-17: rubrica aprovada pela autora, com os pesos (15 pts para cada um dos seis primeiros critérios e 10 para vídeo e one-pager), a divisão Base 10 + Excelência 5 (7 + 3 no último) e a regra de divergência (média; terceiro avaliador se a diferença passar de 15 pts ou se só um acionar eliminatório).
