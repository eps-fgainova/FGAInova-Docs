# Plano de Testes

## Testes End to End
Testes E2E, ou testes de ponta a ponta, são uma metodologia utilizada para verificar se os fluxos de um software funcionam do início ao fim como esperado. Eles simulam o comportamento de um usuário real e avaliam a integração e o desempenho dos componentes do sistema em um ambiente que se assemelha ao máximo com a produção. Isso inclui interações com bancos de dados, redes e APIs, garantindo que tudo funcione de forma coesa e conforme os requisitos definidos.

Os testes E2E são importantes porque ajudam a identificar problemas que podem não ser capturados por testes unitários ou de integração, como falhas de compatibilidade entre diferentes partes do sistema ou erros críticos de desempenho que só aparecem sob condições reais de uso2. Além disso, eles são fundamentais para garantir a segurança, a funcionalidade e a usabilidade do software, proporcionando uma experiência otimizada para o usuário final.

## Behavior-Driven Development e Gherkin
Behavior-Driven Development (BDD) é uma técnica de desenvolvimento ágil que encoraja a colaboração entre desenvolvedores, QA e não-técnicos ou participantes do negócio em um projeto de software. BDD foca em obter uma compreensão clara do comportamento desejado do software através de discussões com stakeholders. Ele estende o TDD (Test-Driven Development) escrevendo casos de teste em uma linguagem natural que não-técnicos podem ler.

Gherkin é uma linguagem de domínio específico que permite descrever o comportamento do software sem detalhar como esse comportamento é implementado. Gherkin é usada para escrever testes automatizados que são compreensíveis por humanos e também por máquinas. A sintaxe de Gherkin é baseada em texto e segue um padrão legível com palavras-chave como “Dado”, “Quando” e “Então”, que definem as condições prévias, a ação a ser testada e o resultado esperado, respectivamente.

Gherkin é frequentemente usado em conjunto com BDD, pois os cenários escritos em Gherkin servem como uma documentação viva que descreve como o software deve se comportar. Eles também são usados como base para os testes de automação.

## Plano de Testes

### FEAT01 - Permitir a criação de uma conta mantenedor

#### **TC01-01** Registro bem-sucedido como mantenedor
<p><strong>Dado</strong> que estou na página de registro de mantenedor</p>
<p><strong>Quando</strong> eu inserir todos os campos obrigatórios corretamente</p>
<p><strong>E</strong> submeter o formulário de registro</p>
<p><strong>Então</strong> uma mensagem de confirmação deve ser exibida</p>

---

#### **TC01-02** Tentativa de registro com campo obrigatório em branco
<p><strong>Dado</strong> que estou na página de registro de mantenedor</p>
<p><strong>Quando</strong> eu deixar um campo obrigatório em branco</p>
<p><strong>Então</strong> o botão de submeter registro estará desabilitado</p>

---

#### **TC01-03** Tentativa de registro com valores inválidos
<p><strong>Dado</strong> que estou na página de registro de mantenedor</p>
<p><strong>Quando</strong> eu deixar um valores inválidos</p>
<p><strong>Então</strong> o botão de submeter registro estará desabilitado</p>

---

#### **TC01-04** Tentativa de registro com valores válidos
<p><strong>Dado</strong> que estou na página de registro de mantenedor</p>
<p><strong>Quando</strong> eu inserir um email que já esteja em uso</p>
<p><strong>E</strong> submeter o formulário de registro</p>
<p><strong>Então</strong> uma mensagem de erro deve ser exibida informando que o email já está em uso</p>

---

### FEAT02 - Permitir a realização a autenticação de sua conta

#### **TC02-01** Login bem-sucedido
<p><strong>Dado</strong> que estou na página de login</p>
<p><strong>Quando</strong> eu inserir um nome de usuário e senha válidos</p>
<p><strong>E</strong> submeter o formulário de login</p>
<p><strong>Então</strong> eu devo ser redirecionado para a página inicial da plataforma</p>

---

#### **TC02-02** Tentativa de Login com dados incorretos
<p><strong>Dado</strong> que estou na página de login</strong>
<p><strong>Quando</strong> eu inserir um <campo> incorreto</strong>
<p><strong>E</strong> submeter o formulário de login</strong>
<p><strong>Então</strong> uma mensagem de erro deve ser exibida informando sobre as credenciais incorretos</strong>
<p>Examples:</p>

| campo |
| ----- |
| email |
| senha |

---

#### **TC02-03** Tentativa de login com campos vazios
<p><strong>Dado</strong> que estou na página de login</p>
<p><strong>Quando</strong> eu não inserir nenhum dado nos campos</p>
<p><strong>Então</strong> o botão de submeter login deve permanecer desabilitado</p>

### FEAT03 - Permitir a criação de uma conta de visitante

#### **TC03-01** Registro bem-sucedido como usuário
<p><strong>Dado</strong> que estou na página de registro de usuário</p>
<p><strong>Quando</strong> eu inserir todos os campos obrigatórios corretamente</p>
<p><strong>E</strong> submeter o formulário de registro</p>
<p><strong>Então</strong> uma mensagem de confirmação deve ser exibida</p>

---

#### **TC03-02** Tentativa de registro com campo obrigatório em branco
<p><strong>Dado</strong> que estou na página de registro de usuário</p>
<p><strong>Quando</strong> eu deixar um campo obrigatório em branco</p>
<p><strong>Então</strong> o botão de submeter registro estará desabilitado</p>

---

#### **TC03-03** Tentativa de registro com valores inválidos
<p><strong>Dado</strong> que estou na página de registro de usuário</p>
<p><strong>Quando</strong> eu deixar um valores inválidos</p>
<p><strong>Então</strong> o botão de submeter registro estará desabilitado</p>

---

#### **TC03-04** Tentativa de registro com valores válidos
<p><strong>Dado</strong> que estou na página de registro de usuário</p>
<p><strong>Quando</strong> eu inserir um email que já esteja em uso</p>
<p><strong>E</strong> submeter o formulário de registro</p>
<p><strong>Então</strong> uma mensagem de erro deve ser exibida informando que o email já está em uso</p>

### FEAT04 - Cadastrar projeto
#### **TC04-01** Cadastro bem-sucedido de um novo projeto
<p><strong>Dado</strong> que estou na página de cadastro de projetos</p>
<p><strong>Quando</strong> eu inserir todas as informações necessárias para o projeto</p>
<p><strong>E</strong> submeter o formulário de cadastro</p>
<p><strong>Então</strong> uma mensagem deve indicar que o cadastro do projeto foi bem sucedido</p>

---

#### **TC04-02** Tentativa de cadastro de projeto com informações incompletas
<p><strong>Dado</strong> que estou na página de cadastro de projetos</p>
<p><strong>Quando</strong> eu não preencher todos os campos obrigatórios</p>
<p><strong>Então</strong> o botão de submeter projeto deve está desabilitado</p>

---

#### **TC04-03** Tentativa de cadastro de projeto com nome já existente
<p><strong>Dado</strong> que estou na página de cadastro de projetos</p>
<p><strong>Quando</strong> eu inserir um nome de projeto que já esteja cadastrado no sistema</p>
<p><strong>E</strong> submeter o formulário de cadastro</p>
<p><strong>Então</strong> uma mensagem de erro deve ser exibida informando que o projeto já existe</p>

---

#### **TC04-04** Acessar projeto
<p><strong>Quando</strong> eu acesso o link de um projeto existente</p>
<p><strong>Então</strong> eu devo ser direcionado para a página de um projeto</p>

---

#### **TC04-05** Tentativa de acessar projeto inexistente
<p><strong>Quando</strong> eu acesso o link de um projeto inexistente</p>
<p><strong>Então</strong> eu devo ser direcionado para a página com uma mensagem indicando projeto não inexistente</p>

<!--   
### FEAT05 - Pesquisar Projeto
### FEAT06 - Curtir Projeto
### FEAT07 - Cadastro de notícias -->



## Bibliografia
>ROCHA, Anne Caroline. Pirâmide de testes e os testes end to end. 25 jan. 2021. Disponível em: <https://medium.com/engenharia-arquivei/t%C3%A9cnicas-de-teste-e2e-64fa50840805>. Acesso em: 07 maio 2024.

>ISMAEL. Desenvolvimento orientado por comportamento (BDD). 2011. Disponível em: <https://www.devmedia.com.br/desenvolvimento-orientado-por-comportamento-bdd/21127>. Acesso em: 07 de maio de 2024.

>BACHION, Julio. O que você precisa saber sobre BDD. 17 mar. 2020. Disponível em: <https://medium.com/join-quality/o-que-voc%C3%AA-precisa-saber-sobre-bdd-70304729d680>. Acesso em: 07 de maio de 2024.

Gherkin Reference. Disponível em: <https://cucumber.io/docs/gherkin/reference/>. Acesso em: 07 de maio de 2024.


### Versionamento

| Versão | Data       | Modificação          | Autor                        | Revisor(es) |
| ------ | ---------- | -------------------- | ---------------------------- | ----------- |
| 1.0    | 23/04/2024 | Criação do Documento | Philipe Serafim e Pedro Lima | Edvan       |