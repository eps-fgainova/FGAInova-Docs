# 1. VISÃO GERAL DO PROJETO

#### 1.1 Organização do Projeto

</br>

| **Papel**     | **Atribuições**                                                                                                                                                                                                                                              | **Responsável** | **Participantes** |
| ------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | --------------- | :---------------: |
| Scrum Master  | O Scrum Master é responsável por garantir que a equipe siga os valores do SCRUM, atua também para remover obstáculos à equipe de desenvolvimento. E ainda junto com o PO será responsável pela organização, planejamento e acompanhamento do projeto.        | Edvan           |  Todos da Equipe  |
| Product Owner | É a pessoa responsável por maximizar o valor resultante do produto desenvolvido. Sua principal responsabilidade é gerenciar o Product Backlog. E ainda junto com o Scrum Master será responsável pela organização, planejamento e acompanhamento do projeto. | Philipe         |  Todos da Equipe  |
| Arquiteto     | É o responsável por liderar e coordenar as atividades e os artefatos técnicos no decorrer do projeto. Implementar os requisitos elicitados, desenvolver as documentações necessárias e escrever testes.                                                      | Pedro Lima      |  Todos da Equipe  |



# 2. Ferramentas, Ambiente e Infraestrutura

### 2.1. Hardware

| **Perfil**                 | **Tipo de Hardware** | **Configurações**        | **Qtd. Planejada(es)** | **Prazo Estimado** | **Observação** |
| -------------------------- | :------------------: | ------------------------ | :--------------------: | :----------------: | :------------: |
| Todos os perfis planejados |      Computador      | i5 5ª geração 8GB de Ram |           03           |         -          |       -        |

### 2.1. Software

| **Perfil**                 | **Tipo de Software**                                | **Nome da Ferramenta** | **Versão** | **Qtd Licenças Planejada** | **Prazo Estimado** |
| -------------------------- | --------------------------------------------------- | ---------------------- | :--------: | :------------------------: | :----------------: |
| Todos os perfis planejados | Ferramenta de versionamento de código               | Git                    |  ~ 2.25.1  |             -              |         -          |
| Todos os perfis planejados | Repositório para código e documentação              | GitLab                 |     -      |             -              |         -          |
| Devops                     | Pipeline de CI/CD                                   | GitLab                 |     -      |             -              |         -          |
| Todos os perfis planejados | Compartilhamento de arquivos                        | Google Drive           |     -      |             -              |         -          |
| Todos os perfis planejados | Editor de código-fonte                              | Visual Studio Code     |   ~1.58    |             -              |         -          |
| Todos os perfis planejados | Cliente desktop API para Rest e GraphQL             | Postman                |  ~ 8.9.1   |             -              |         -          |
| Todos os perfis planejados | Plataforma de gestão de tarefas                     | Trello                 |     -      |             -              |         -          |
| Todos os perfis planejados | Ferramenta de comunicação do time e envio de avisos | Telegram               |  ~ 2.8.8   |             -              |         -          |
| Todos os perfis planejados | Aplicativo para comunicação síncrona                | Discord                |     -      |             -              |         -          |
| Todos os perfis planejados | Plataforma de quadro branco colaborativo            | Figma                  |     -      |             -              |         -          |
| Todos os perfis planejados | Implementação de virtualização de containers        | Docker                 |     -      |             -              |         -          |
| Todos os perfis planejados | Plataforma de nuvem                                 | Amazon Web Services    |     -      |             -              |         -          |

# 3. Processo de Gerência de Projeto

## 3.1 Processo de Desenvolvimento e Mensuração

### 3.1.1 Metodologia do Projeto

<p>O time optou por adotar uma combinação do Scrum e do XP. Essa decisão foi tomada através da análise de fatores técnicos, organizacionais e humanos.</p>
<p>Olhando para os aspectos humanos, o Scrum e XP são as melhores alternativas de desenvolvimento e trabalho pela experiência que os membros do time têm com essas metodologias com base na experiência adquirida na matéria de Métodos de Desenvolvimento de Software (MDS) e por todos participarem do contexto da Empresa Júnior de Engenharia de Software.</p>
<p>Já observando os aspectos em um viés mais organizacional, outro motivo para essa decisão foi a maneira como a matéria é estruturada em diversas entregas através de um mínimo produto viável (MVP). Essa configuração torna propício o desenvolvimento do produto em ciclos ágeis.</p>
<p>Por fim, traçando o panorama técnico, percebe-se que o projeto possui um escopo grande, por isso a metodologia de construção envolve o uso de MVPs. Nesse sentido, a escolha de Scrum e XP mostra-se mais adequada, para garantir a adaptabilidade do projeto à medida que incrementamos na entrega dos MVPs.</p>
<p>Durante o desenvolvimento do projeto serão realizadas reuniões diárias de 10 minutos no formato proposto pela metodologia Scrum. Também selecionamos o prazo de 7 dias (uma semana) para a Sprint do projeto. Essa escolha se deve por englobar tempo suficiente para o time realizar suas execuções, fechando o ciclo no domingo com retrospectiva e planejamento. Além de permitir que o time valide mais rápido entre si as atividades da sprint e esteja acompanhando o progresso como um grupo, esse período de sete dias está em consonância com o ritmo e volume de entrega das unidades da disciplina, uma vez que precisamos de iterações mais constantes para validações.</p>
<p>No final de cada sprint, que neste projeto corresponde ao tempo de uma semana, é realizada uma reunião de retrospectiva da sprint com duração de 2 horas aos domingos, onde o progresso do time é revisado com base nos gráficos de Fluxo Cumulativo, BurnUp do projeto e Velocidade de Desenvolvimento, incluindo também a análise e gerenciamento de riscos. Além disso, nessa reunião é iniciado o próximo ciclo, onde cada tarefa deve ser estimada dentro do contexto do Planning Poker, usando a sequência de Fibonacci para avaliar a dificuldade de cada atividade a ser concluída.</p>

### 3.1.2 Metodologia de Elicitação de Requisitos

<p>Foi utilizado o Lean Inception para identificar os requisitos essenciais, promovendo uma diversidade de ideias para o escopo do FGAInova e testando as características funcionais do sistema.</p>

<p>Após a Lean Inception, o time tinha em mãos os requisitos do projeto e precisava de um método para documentação e detalhamento. Assim, adotamos o Modelo de Canvas MVP, que, em conjunto com a Lean Inception, nos ofereceu uma perspectiva do usuário, clareza nas interfaces do produto e critérios de aceitação bem definidos. Além disso, o Modelo de Canvas MVP destacou o valor de negócio dos requisitos para os clientes.</p>

### 3.1.3 Walkthrough

<p>Uma técnica de validação muito importante para a construção do nosso backlog foi o Walkthrough. Essa técnica foi amplamente utilizada pela equipe em vários momentos na validação dos requisitos elicitados — para garantir que os requisitos estavam sendo feitos da maneira correta e desenhando o produto certo. A escolha dessa técnica ocorreu porque ela é mais flexível e simples, uma vez que pode ser feita em reuniões informais e sem preparação do time, tendo por objetivo conseguir a aprovação dos envolvidos para seguir com o projeto.</p>
<p>Outra técnica que utilizamos foi as etapas de inspeção, em geral todos os membros da equipe exerceram todos os papéis. No levantamento de ideias todos participaram validando o que foi sugerido e escrito. Não tivemos um papel fixo de coordenador das inspeções, pois avaliamos juntos os processos realizados. Os erros levantados, como uma história desnecessária, serão corrigidos e as sugestões debatidas em equipe, antes de partir para a implementação. Escolhemos esse método porque trazia mais agilidade às reuniões, participação e opinião de todos os membros, não tendo um tempo de espera além do já ocorrido na reunião.

### 3.1.4 Documentação e Gerenciamento

<p>Para efetuar a documentação foi escolhida a elaboração de uma wiki por meio de repositório no gitlab usando o framework docsify como gerenciamento da documentação do projeto. Essa escolha se dá pelo fato do framework permitir a elaboração de documentações de forma organizada em com usabilidade eficiente. Por meio do próprio gitlab é disponibilizada a documentação pelo gitlab pages. O controle de versionamento é feito pelas tabelas presentes em cada artigo e página da documentação.</p>

### Versionamento

| Versão | Data       | Modificação          | Autor           | Revisor(es) |
| ------ | ---------- | -------------------- | --------------- | ----------- |
| 1.0    | 23/04/2024 | Criação do Documento | Philipe Serafim | Pedro Lima  |