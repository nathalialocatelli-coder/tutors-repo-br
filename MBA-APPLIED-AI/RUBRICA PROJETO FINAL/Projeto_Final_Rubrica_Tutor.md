# Projeto Final · Rubrica do Tutor

**Uso interno. Não compartilhar com o aluno.**
Componente 12 · Caso Aplicado Integrado · versão 1

O aluno recebe o enunciado e a tabela de critérios com os quatro níveis descritos. Este documento é o que fica no repositório do tutor: pontuação exata, onde olhar em cada entrega, gabarito analítico dos casos, conjunto selado de entradas, sinais de fraude, roteiro de banca e modelo de devolutiva.

## O que é aberto e o que é restrito

| Material | Aluno | Tutor |
|---|---|---|
| Enunciado, peças e formato de entrega | sim | sim |
| Tabela de critérios com descritores dos quatro níveis | sim | sim |
| Pontuação exata de cada nível | não | sim |
| Conjunto selado de 10 entradas de teste por caso | não | sim |
| Conta de custo de referência por caso | não | sim |
| Gabarito analítico dos casos | não | sim |
| Sinais de fraude e procedimento | não | sim |
| Regras de reconciliação entre avaliadores | não | sim |

O aluno sabe **o que** é avaliado e **como** se descreve cada nível. Ele não sabe quanto vale cada nível, nem quais entradas serão sorteadas, nem qual é a resposta esperada do caso.

## Fluxo de correção

1. **Antes da banca**, o tutor lê o dossiê, o registro de testes e o one-pager, e preenche os critérios 1, 2, 4, 5 e 6. Tempo estimado: 25 minutos.
2. **Na banca**, avalia o critério 3, protótipo, com a entrada sorteada, e o critério 7, defesa. Tempo: os 15 minutos da apresentação.
3. **Logo após**, os dois avaliadores lançam nota independente antes de conversar entre si.
4. **Reconciliação**, obrigatória quando a diferença passa de 8 pontos no total ou de um nível em qualquer critério.
5. **Devolutiva ao aluno** em até 5 dias úteis, no modelo do fim deste documento.

📌 Lançar nota antes da conversa é o que impede o avaliador mais seguro de arrastar o outro.

## Pontuação por critério

Quatro níveis: Ausente, Insuficiente, Suficiente, Excelente.

| Critério | Peso | Ausente | Insuficiente | Suficiente | Excelente |
|---|---|---|---|---|---|
| 1. Diagnóstico e enquadramento | 15 | 0 | 6 | 11 | 15 |
| 2. Desenho da solução | 15 | 0 | 6 | 11 | 15 |
| 3. Protótipo funcional | 20 | 0 | 8 | 14 | 20 |
| 4. Governança e risco | 15 | 0 | 6 | 11 | 15 |
| 5. Métricas e evidência | 15 | 0 | 6 | 11 | 15 |
| 6. Conta de operação | 10 | 0 | 4 | 7 | 10 |
| 7. Defesa e one-pager | 10 | 0 | 4 | 7 | 10 |

**Nota mínima de aprovação:** 60 pontos, mais nenhum eliminatório acionado.

**Reentrega:** uma única vez, em 15 dias, com teto de 70 pontos.

## Como avaliar cada critério

### 1. Diagnóstico e enquadramento · 15

**Onde olhar:** bloco 1 do dossiê e os dois primeiros minutos da defesa.

**Ausente:** o problema aparece só em adjetivos, sem número algum.
**Insuficiente:** há número, mas ele não vem do caso ou não tem origem declarada.
**Suficiente:** há pelo menos um número do caso, com origem.
**Excelente:** o número tem linha de base, e a escolha do processo é justificada contra alternativas descartadas.

**Não conta como justificativa:** "foi o processo mais crítico", sem critério. Conta: comparação pelos três eixos, ou pela restrição do caso.

### 2. Desenho da solução · 15

**Onde olhar:** bloco 3 do dossiê, com diagrama, e o que o protótipo de fato faz.

**Ausente:** não dá para dizer o que o sistema faz lendo o dossiê.
**Insuficiente:** fluxo descrito, sem separar o que é automação, agente e humano.
**Suficiente:** a separação existe e está clara.
**Excelente:** a separação é justificada por tolerância ao erro e volume, e o diagrama é legível sem narração.

**Atenção:** desenho que entrega ao modelo uma tarefa determinística, como calcular desconto ou buscar preço em tabela, não passa de Insuficiente neste critério, por melhor que esteja escrito.

### 3. Protótipo funcional · 20

**Onde olhar:** demonstração na banca, instrução de sistema e pacote do protótipo.

**Ausente:** não roda, ou não existe caminho de disparo manual.
**Insuficiente:** roda apenas no caminho feliz ensaiado pelo aluno.
**Suficiente:** acerta 2 de 3 entradas cegas sem travar, com instrução de sistema documentada.
**Excelente:** acerta 3 de 3, e o guardrail dispara com mensagem rastreável na entrada construída para quebrá-lo.

**Na entrada sorteada, pontua o comportamento, não o acerto.** Escalar para humano, declarar baixa confiança ou recusar conta como acerto. Inventar resposta plausível com número errado conta como erro, mesmo que a formatação esteja perfeita.

### 4. Governança e risco · 15

**Onde olhar:** bloco 4 do dossiê e a resposta à segunda pergunta obrigatória.

**Ausente:** risco genérico do tipo "a IA pode errar", sem mitigação.
**Insuficiente:** registro preenchido, com mitigação que não se sustenta.
**Suficiente:** risco principal nomeado corretamente, com mitigação e responsável.
**Excelente:** a mitigação sobrevive à conta de volume, e a restrição do caso é respeitada no desenho, não só mencionada.

**Teste da conta de volume:** se a mitigação é revisão humana, divida o volume do caso pelo tempo da equipe informado pelo aluno. Abaixo de dois minutos por item, a mitigação não se sustenta e o critério não passa de Suficiente.

### 5. Métricas e evidência · 15

**Onde olhar:** bloco 5 do dossiê e o registro de testes.

**Ausente:** não há métrica, ou o registro de testes não existe.
**Insuficiente:** métrica sem linha de base, **ou registro com 100% de acerto**.
**Suficiente:** métrica de resultado com linha de base e registro de testes real.
**Excelente:** há métrica de qualidade como contrapeso, e pelo menos um erro do protótipo está relatado com o que foi feito a respeito.

‼️ Registro sem nenhum erro é, na prática, registro não feito.

### 6. Conta de operação · 10

**Onde olhar:** bloco 6 do dossiê, planilha anexa e a primeira pergunta obrigatória.

**Ausente:** não há conta.
**Insuficiente:** número sem premissa declarada, ainda que correto.
**Suficiente:** memória de cálculo com volume do caso e custo unitário declarado.
**Excelente:** inclui custo de revisão humana e identifica a variável que mais move o custo.

**O avaliado é a memória de cálculo, não o resultado.** Qualquer valor dentro de 30% da conta de referência do caso, com premissas explícitas, vale Excelente.

### 7. Defesa e one-pager · 10

**Onde olhar:** os 15 minutos e o one-pager público.

**Ausente:** estoura o tempo sem demonstrar, ou não entregou one-pager.
**Insuficiente:** demonstra, mas responde as perguntas obrigatórias sem número.
**Suficiente:** cabe no tempo, demonstra e responde as três perguntas.
**Excelente:** responde com número, inclusive a de custo, e o one-pager se sustenta fora do curso, sem depender do contexto da escola.

## Gabarito analítico dos casos

Não é resposta única. É o que uma entrega Excelente precisa ter enfrentado.

### Caso A · Clínicas

A entrega boa separa os identificadores do corpo da mensagem **antes** da ferramenta nova, trata só a categoria sem dado sensível e deixa explícito o que fica com humano por natureza do dado.

**Erro esperado:** tratar as três categorias no mesmo fluxo e mencionar a restrição no dossiê sem refleti-la no desenho. Isso trava o critério 4 em Suficiente, no máximo.

**Guardrail natural:** mascaramento ou remoção do identificador antes do envio.

### Caso B · Distribuidora

A entrega boa identifica o item com o modelo e **busca o preço e calcula o desconto fora dele**, em passo determinístico. A conta de operação precisa fechar em 1,25 real por cotação, considerando as chamadas por execução, não uma só.

**Erro esperado:** deixar a tabela de 300 itens no contexto ou numa base vetorial e pedir o preço ao modelo. Gera o erro silencioso do item vizinho e trava o critério 2.

**Conta de referência:** *a preencher quando o pacote de dados do caso estiver pronto, com distribuição de itens por pedido e tamanho do catálogo em tokens.*

### Caso C · Contábil

A entrega boa declara a **taxa de erro residual aceita** e a defende contra o custo da multa, propondo revisão por faixa de criticidade fiscal, e não revisão de tudo nem amostragem uniforme.

**Erro esperado:** propor revisão humana de 100% sem relacionar com o valor da multa e com a taxa de erro atual dos analistas. Note que a conta de tempo fecha, então a resposta não é errada por capacidade: ela é incompleta por não tratar risco.

**Guardrail natural:** limiar de confiança que roteia para humano.

## Conjunto selado de entradas

Cada caso tem 10 entradas, custodiadas pelo tutor: 6 normais, 2 ambíguas e 2 que devem ser recusadas ou escaladas pelo guardrail.

Na banca, sorteie **uma** entre as 10, evitando repetir a mesma entrada para dois alunos seguidos do mesmo caso.

*Conjuntos a produzir junto com os casos. Formato: arquivo por caso, com a entrada, o comportamento esperado e o que caracteriza erro.*

Em caso próprio, o conjunto é proposto pelo aluno ao fim da etapa 2 e selado pelo tutor. Se o aluno não entregou o conjunto, o caso próprio não foi aprovado e a entrega é avaliada como caso da escola não realizado.

## Sinais de fraude e de fachada

Nenhum deles reprova sozinho, com exceção do último. Todos pedem pergunta adicional na banca.

**Protótipo de fachada.** Acerta as três entradas do aluno e trava na primeira entrada sorteada. Pergunte como ele testou e o que mudou entre a primeira e a última versão.

**Números redondos demais.** Redução de exatamente 50%, economia de exatamente 10 mil reais. Peça a memória de cálculo na hora.

**Registro de testes perfeito.** Critério 5 não passa de Insuficiente, por regra.

**Dossiê genérico.** Texto que serviria para qualquer caso, sem número do pacote de dados entregue. Verifique se os números citados existem no CSV do caso.

**Declaração de uso de IA ausente.** Eliminatório.

**Dado real identificável na entrega.** Eliminatório, com registro para a coordenação.

## Eliminatórios

| Situação | Procedimento |
|---|---|
| Protótipo não verificável | Antes de eliminar, confirme as três formas de verificação: ao vivo, vídeo com execução contínua e horário visível, ou execução pela banca em até 48 horas |
| Declaração de uso de IA ausente | Comunicar ao aluno e abrir prazo de 48 horas para envio, antes de eliminar |
| Dado real identificável de cliente ou paciente | Eliminatório imediato, com comunicação à coordenação |

**Falha de infraestrutura na banca não elimina.** Converta para a gravação e mantenha a arguição integral, incluindo a entrada sorteada, pedindo ao aluno que descreva o comportamento esperado antes de rodar o vídeo.

## Roteiro da banca

| Tempo | Bloco | O que observar |
|---|---|---|
| 0 a 2 min | Problema em número | Critério 1 |
| 2 a 3 min | Oportunidade e descartadas | Critério 1 |
| 3 a 9 min | Demonstração, com a entrada sorteada | Critério 3 |
| 9 a 11 min | Risco e o que fica humano | Critério 4 |
| 11 a 13 min | Conta de operação e métricas | Critérios 5 e 6 |
| 13 a 15 min | Arguição | Critério 7 |

**As três perguntas obrigatórias**, feitas a todos:

1. Quanto custa operar isso no volume real do caso, e como você chegou a esse número?
2. O que acontece quando a solução erra, e quem percebe antes do cliente?
3. Por que não resolver com automação simples?

**Como pontuar as respostas.** Resposta com número e premissa conta para Excelente no critério 7. Resposta correta sem número conta Suficiente. "Fica barato, uns centavos por chamada" conta Insuficiente.

A quarta pergunta fica a critério da banca, dirigida ao ponto mais frágil da apresentação. Registre qual foi, para a devolutiva.

## Modelo de devolutiva

Três blocos, de três a cinco linhas cada, enviados em até 5 dias úteis.

**O que sustentou a entrega.** O ponto mais forte, nomeando o critério.

**O que custou pontos.** Os dois achados de maior peso, com o nível atribuído e o que faltava para o nível seguinte. Específico: "a conta de operação não declarou chamadas por execução, o que mantém o critério em Suficiente".

**O que fazer com isso fora do curso.** Uma recomendação prática sobre o one-pager ou sobre o próximo passo da solução, considerando que o aluno vai mostrar isso em outro lugar.

## Pendências desta rubrica

**Conjuntos selados de entradas**, três arquivos, a produzir com os casos.

**Contas de referência de custo**, uma por caso, a fechar quando os dados estiverem definidos.

**Nota mínima e política de reentrega**, a confirmar com a coordenação.

**Formato do repositório.** Este documento está em markdown, pronto para o repositório do tutor. Se houver padrão definido para rubricas de outras sprints, alinhar nomes de arquivo e estrutura de pastas antes de publicar.
