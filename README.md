Miniguia de Estudos — Agentes de Inteligência Artificial com NotebookLM
Sobre o Projeto
Este projeto foi desenvolvido como parte de um desafio prático da DIO, utilizando o NotebookLM como ferramenta de aprendizagem ativa.
O tema escolhido foi Agentes de Inteligência Artificial. O objetivo do estudo é compreender o que são agentes de IA, como funcionam, quais são seus principais componentes e como modelos de linguagem, memória, planejamento e ferramentas externas podem trabalhar juntos para executar tarefas.
Além do aprendizado sobre agentes de IA, o projeto busca explorar técnicas de curadoria de fontes e engenharia de prompts, analisando como diferentes instruções fornecidas à IA podem influenciar a qualidade e a profundidade das respostas.
Objetivos de Estudo
- Compreender o conceito de agente de inteligência artificial.
- Identificar as diferenças entre agentes, workflows, assistentes e bots.
- Entender o papel dos modelos de linguagem (LLMs) dentro de um agente.
- Compreender conceitos como memória, planejamento e ferramentas externas.
- Entender o funcionamento de Tool Calling.
- Explorar o conceito de Human-in-the-Loop.
- Observar como um agente pode executar tarefas através de ciclos de raciocínio e ação.
- Praticar engenharia de prompts utilizando o NotebookLM.
Curadoria de Fontes
Foram selecionadas quatro fontes técnicas e educacionais para construir a base de conhecimento utilizada no NotebookLM.
1. Google Cloud Tech — Building AI Agents on Google Cloud
https://www.youtube.com/watch?v=8rlNdKywldQ
Vídeo técnico utilizado para complementar o estudo com uma perspectiva prática sobre a construção e o funcionamento de agentes de IA.
2. Anthropic — Building Effective Agents
https://www.anthropic.com/engineering/building-effective-agents
Material técnico utilizado para aprofundar o estudo sobre construção de agentes, workflows e padrões utilizados em sistemas baseados em modelos de linguagem.
3. Microsoft Learn — Introduction to AI Agents
https://learn.microsoft.com/en-us/startups/build/ai/agents/intro-agents
Documentação introdutória utilizada para compreender a estrutura, os componentes e o funcionamento dos agentes de inteligência artificial.
4. Google Cloud — What are AI agents?
https://cloud.google.com/discover/what-are-ai-agents
Material utilizado para estudar conceitos, características e fundamentos relacionados aos agentes de inteligência artificial.
Engenharia de Prompts e Cicatrizes
Durante o estudo, diferentes prompts foram utilizados no NotebookLM para observar como alterações nas instruções modificavam as respostas geradas.
Prompt 1 — Exploração Inicial
Prompt utilizado:
Com base exclusivamente nas fontes fornecidas, explique o que é um agente de inteligência artificial, como ele funciona e quais são seus principais componentes.

Resultado
O NotebookLM apresentou uma resposta estruturada contendo:
- definição de agente de IA;
- diferenças entre agentes, workflows, assistentes e bots;
- ciclo de percepção, raciocínio e ação;
- Tool Calling;
- Human-in-the-Loop;
- modelos de linguagem;
- ferramentas externas;
- memória.
Cicatriz Encontrada
A resposta apresentou corretamente os conceitos fundamentais, porém permaneceu predominantemente conceitual.
Mesmo compreendendo individualmente conceitos como LLM, memória, planejamento e ferramentas, ainda não ficava totalmente evidente como esses elementos poderiam trabalhar juntos durante a execução de uma tarefa real.
Essa limitação levou à elaboração de um segundo prompt, solicitando explicitamente uma aplicação prática.
Prompt 2 — Aplicação Prática
Prompt utilizado:
Com base exclusivamente nas fontes fornecidas, explique o que é um agente de inteligência artificial e seus principais componentes. Em seguida, demonstre o funcionamento completo através de um exemplo prático de um agente que busca vagas de emprego para um usuário. Mostre passo a passo quando o agente utiliza o modelo de linguagem, memória, planejamento e ferramentas externas. Ao final, indique quais fontes sustentam cada parte da explicação.

Resultado
A segunda resposta apresentou um cenário prático de funcionamento de um agente responsável por buscar vagas de emprego.
O fluxo apresentado pode ser resumido como:
Usuário → LLM e Memória → Planejamento → Ferramentas/APIs → Resultados → Reavaliação → Supervisão Humana → Ação Final
No exemplo, o agente:
1. recebe o objetivo do usuário;
2. interpreta a solicitação;
3. consulta informações e preferências armazenadas;
4. divide o objetivo em etapas;
5. utiliza ferramentas externas para buscar vagas;
6. analisa os resultados encontrados;
7. compara as oportunidades com o perfil profissional;
8. solicita autorização antes de executar uma ação importante;
9. executa a ação autorizada;
10. registra informações relevantes para consultas futuras.
Melhoria Observada
A inclusão de um cenário prático tornou mais clara a relação entre os diferentes componentes de um agente.
Enquanto o primeiro prompt foi eficiente para apresentar os conceitos, o segundo permitiu visualizar como LLM, memória, planejamento e ferramentas externas trabalham em conjunto durante a execução de uma tarefa.
O experimento demonstrou que fornecer contexto, definir o objetivo da resposta e solicitar um formato específico pode tornar a interação com a IA mais útil para o processo de aprendizagem.
Miniguia de Estudo
1. O que é um Agente de IA?
Um agente de inteligência artificial é um sistema de software orientado a objetivos que utiliza um modelo de linguagem como parte central de seu processo de raciocínio, planejamento, tomada de decisões e execução de tarefas.
Diferentemente de sistemas tradicionais baseados apenas em regras fixas, um agente pode analisar o ambiente, utilizar ferramentas externas e adaptar suas próximas ações de acordo com os resultados encontrados.
2. Agentes, Workflows, Assistentes e Bots
Uma das principais diferenças entre essas abordagens está no grau de autonomia e flexibilidade.
Bot
Possui baixa autonomia e normalmente executa ações baseadas em regras previamente programadas.
Assistente de IA
Interage com o usuário e auxilia na realização de tarefas, mas normalmente depende da participação e das decisões do usuário.
Workflow
Segue uma sequência previamente definida de etapas. É adequado quando o processo é conhecido e previsível.
Agente de IA
Possui maior autonomia. O modelo pode decidir dinamicamente quais passos executar, quais ferramentas utilizar e como adaptar seu plano conforme os resultados obtidos.
De forma simplificada:
Workflow = caminho previamente definido.
Agente = caminho decidido dinamicamente durante a execução.
3. Principais Componentes de um Agente
Modelo de Linguagem (LLM)
Atua como o motor de inteligência do agente, permitindo interpretar linguagem, analisar informações e auxiliar na tomada de decisões.
Instruções e Objetivos
Definem o papel do agente, suas metas, regras, restrições e comportamento esperado.
Ferramentas (Tools)
Permitem que o agente interaja com sistemas externos.
Alguns exemplos:
- APIs;
- bancos de dados;
- mecanismos de busca;
- navegadores;
- calculadoras;
- ambientes de execução de código.
Memória
Permite ao agente manter informações relevantes sobre a tarefa ou sobre interações anteriores.
Ela pode ser dividida em:
- Memória de curto prazo: mantém o contexto da tarefa ou conversa atual.
- Memória de longo prazo: armazena informações persistentes, históricos e preferências para utilização futura.
Planejamento
Permite decompor objetivos complexos em tarefas menores e decidir quais ações devem ser executadas para alcançar determinado resultado.
4. Ciclo de Funcionamento de um Agente
O funcionamento de um agente pode ser representado de maneira simplificada pelo seguinte fluxo:
Objetivo → Raciocínio → Planejamento → Ferramenta → Resultado → Avaliação → Próxima Ação
Etapa 1 — Recepção do Objetivo
O usuário fornece uma tarefa ou objetivo.
Etapa 2 — Raciocínio e Planejamento
O agente interpreta o objetivo e determina quais etapas podem ser necessárias.
Etapa 3 — Tool Calling
Quando precisa de informações ou ações externas, o agente seleciona e chama uma ferramenta.
Etapa 4 — Retorno do Ambiente
A ferramenta fornece o resultado da ação realizada.
Etapa 5 — Avaliação
O agente analisa o resultado obtido.
Caso o objetivo ainda não tenha sido alcançado, ele pode ajustar seu plano e executar outra ação.
Caso o objetivo tenha sido alcançado, o agente apresenta o resultado final.
5. Tool Calling
Tool Calling é a capacidade de um modelo identificar quando precisa utilizar uma ferramenta externa para continuar uma tarefa.
Por exemplo, um agente responsável por encontrar vagas de emprego não possui necessariamente informações atualizadas sobre vagas abertas.
Nesse caso, ele pode utilizar uma API ou ferramenta de busca para obter dados atuais e posteriormente analisar os resultados encontrados.
6. Memória
A memória permite que um agente mantenha contexto e utilize informações relevantes durante suas decisões.
Memória de Curto Prazo
Armazena informações relacionadas à tarefa ou conversa atual.
Memória de Longo Prazo
Permite armazenar informações persistentes, como:
- preferências;
- histórico de ações;
- interações anteriores;
- informações relevantes sobre o usuário.
7. Planejamento e Auto-Refinamento
Um agente pode decompor uma tarefa complexa em etapas menores.
Além disso, pode analisar os resultados obtidos durante a execução e modificar sua estratégia.
Se uma ferramenta retornar um erro ou um resultado inadequado, por exemplo, o agente pode ajustar seus parâmetros ou escolher outra abordagem.
Essa capacidade permite que o sistema tenha maior flexibilidade durante a execução.
8. Autonomia e Human-in-the-Loop
Apesar da capacidade de executar tarefas autonomamente, nem todas as decisões devem ser realizadas sem supervisão.
O conceito de Human-in-the-Loop adiciona pontos de controle onde uma pessoa pode revisar ou autorizar determinadas ações.
Por exemplo, um agente pode:
1. pesquisar vagas;
2. analisar as melhores oportunidades;
3. preparar uma candidatura;
4. solicitar autorização do usuário;
5. somente então enviar a candidatura.
Isso permite combinar automação com supervisão humana em ações importantes.
Glossário
Agente de IA (AI Agent)
Sistema de software orientado a objetivos que utiliza inteligência artificial para raciocinar, planejar e executar tarefas com determinado grau de autonomia.
LLM (Large Language Model)
Modelo de linguagem de grande escala que pode atuar como motor de raciocínio e compreensão de linguagem de um agente.
Workflow
Fluxo de trabalho no qual uma sequência de etapas é previamente definida.
Tool Calling
Capacidade do modelo de identificar a necessidade de utilizar uma ferramenta externa e gerar uma chamada apropriada para ela.
Tools
Ferramentas externas que ampliam as capacidades do agente, como APIs, bancos de dados, navegadores e ambientes de execução de código.
Memória de Curto Prazo
Informações mantidas durante a tarefa ou interação atual.
Memória de Longo Prazo
Armazenamento persistente de informações que podem ser utilizadas em interações futuras.
Planejamento (Planning)
Processo de decompor um objetivo em etapas e decidir quais ações executar.
Human-in-the-Loop
Modelo de operação no qual uma pessoa participa de determinados pontos do processo para revisar, orientar ou autorizar ações.
API (Application Programming Interface)
Interface que permite a comunicação e troca de informações entre diferentes sistemas e aplicações.
RAG (Retrieval-Augmented Generation)
Técnica que permite recuperar informações de fontes externas e fornecê-las ao modelo para auxiliar na geração de respostas fundamentadas.
Ground Truth
Informação factual obtida do ambiente ou de uma ferramenta utilizada pelo agente durante sua execução.
Prompts Reutilizáveis
Os prompts abaixo foram criados para permitir futuras revisões do conteúdo utilizando as fontes presentes no NotebookLM.
1. Revisão Conceitual
Com base nas fontes do caderno, faça uma explicação detalhada sobre o conceito de [INSERIR CONCEITO]. Explique o que é, por que esse componente é importante na construção de um agente e apresente um exemplo prático de como ele atua durante a execução.

2. Comparação de Tecnologias e Arquiteturas
Com base no material salvo, compare [TECNOLOGIA OU ABORDAGEM A] com [TECNOLOGIA OU ABORDAGEM B]. Monte uma tabela destacando nível de autonomia, previsibilidade, complexidade de implementação e cenário ideal de utilização.

3. Quiz de Fixação
Com base exclusivamente nas fontes deste caderno, crie um quiz de 5 perguntas de múltipla escolha para testar meus conhecimentos sobre [INSERIR TEMA]. Não mostre as respostas imediatamente. Aguarde minhas respostas e depois apresente o gabarito com uma explicação para cada questão.

4. Estudo de Caso
Com base nas boas práticas apresentadas pelas fontes, desenvolva o passo a passo de um agente de IA para solucionar o seguinte problema: [DESCREVER PROBLEMA]. Indique o papel do LLM, quais ferramentas externas seriam utilizadas, como a memória poderia ser estruturada e em quais momentos seria necessária supervisão humana.

5. Troubleshooting
Com base nas fontes, analise o seguinte problema apresentado por um agente: [DESCREVER FALHA]. Explique possíveis causas e sugira ajustes no prompt, planejamento, ferramentas ou tratamento de erros para corrigir o comportamento.

6. Comparação entre as Fontes
Com base nas fontes da Anthropic, Microsoft e Google Cloud utilizadas neste caderno, analise como cada organização aborda [INSERIR TEMA]. Identifique os principais pontos de concordância e as diferenças entre as abordagens.

Ferramentas Utilizadas
- NotebookLM
- GitHub
- Markdown
- Inteligência Artificial Generativa
Conclusão
O desenvolvimento deste projeto permitiu utilizar o NotebookLM como ferramenta de aprendizagem baseada em fontes selecionadas previamente.
A curadoria de materiais de diferentes organizações possibilitou estudar agentes de inteligência artificial a partir de perspectivas distintas, enquanto os testes de prompts demonstraram como alterações na formulação de uma pergunta podem modificar a profundidade e a aplicabilidade das respostas.
A principal evolução observada ocorreu entre o primeiro e o segundo prompt. Enquanto a primeira consulta apresentou os conceitos de maneira predominantemente teórica, a inclusão de um cenário prático permitiu compreender melhor como LLM, memória, planejamento e ferramentas externas podem trabalhar em conjunto.
Além do conteúdo sobre agentes de IA, o projeto proporcionou experiência prática com curadoria de fontes, engenharia de prompts, análise crítica das respostas e organização de conhecimento utilizando inteligência artificial.