# Desafio: Sistema de Gerenciamento de Tarefas

## Descrição
Desenvolva um sistema de gerenciamento de tarefas utilizando NextJS. O sistema deve permitir que os usuários se registrem, façam login, criem, editem e excluam tarefas. A autenticação deve ser feita via Auth0 e todas as operações de tarefas devem ser protegidas, exigindo um token de autenticação válido.

## Requisitos

1. **Autenticação via Auth0:**
   - Configurar autenticação de usuários utilizando Auth0.
   - Implementar o fluxo de login e logout.
   - Proteger rotas para que apenas usuários autenticados possam acessar a área de gerenciamento de tarefas.

2. **Gerenciamento de Tarefas:**
   - Implementar CRUD (Create, Read, Update, Delete) de tarefas.
   - Cada tarefa deve ter os seguintes campos:
     - Título
     - Descrição
     - Data de criação
     - Status (Pendente, Em andamento, Concluída)
   - Permitir que os usuários visualizem apenas as suas próprias tarefas.

3. **API Backend:**
   - Utilize uma API mock como JSONPlaceholder (https://jsonplaceholder.typicode.com/) para simular o backend.
   - As chamadas à API devem ser autenticadas utilizando o token de autenticação obtido via Auth0.

4. **Capacidades Avançadas de NextJS:**
   - Utilização de Server-Side Rendering (SSR) para melhorar a performance e SEO.
   - Implementação de rotas dinâmicas para visualizar e editar tarefas.
   - Utilização de `getServerSideProps` ou `getStaticProps` conforme necessário.
   - Boa organização de código, com componentes reutilizáveis e uso de hooks personalizados quando aplicável.
   - Testes unitários com bibliotecas de escolha do candidato (ver lista abaixo).
   - Boa documentação do código e um README claro explicando como configurar e rodar o projeto.

### Bibliotecas Recomendadas:
- `react-hook-form`: Utilize para gerenciar formulários de maneira eficiente.
- Tanstack Query (react-query): Utilize para gerenciar o estado da busca de dados e cache de maneira otimizada e escalável.
- Tailwind CSS: Utilize Tailwind CSS para estilização da aplicação de forma rápida e eficiente.

### Regras de Formatação e Controle de Qualidade:
- Prettier: Configurar regras de formatação com Prettier e garantir que o código segue um estilo consistente.
- Husky: Configurar Husky para adicionar ganchos de Git, garantindo que o código esteja formatado corretamente e passe por verificações antes de ser comitado.

### Performance e Otimização:
- Uso de técnicas de otimização para melhorar a performance da aplicação.

### Internacionalização (i18n):
- Suporte para múltiplos idiomas utilizando bibliotecas adequadas.

### Gerenciamento de Estado:
- Uso eficiente de gerenciamentos de estado global e local.

### Manutenibilidade e Extensibilidade:
- Estrutura do projeto organizada e modular.
- Documentação de código clara e adequada.

### [Plus] Integração Contínua e Entrega Contínua (CI/CD):
- Configuração de pipelines de CI/CD.
- Automação de testes e deploy contínuo.

### [Plus] Acessibilidade:
- Aderência aos padrões de acessibilidade.
- Funcionalidade adequada com navegação via teclado e leitores de tela.

## Telas da Aplicação

### Tela de Login
**Layout:**
- Formulário de login centralizado na tela.
- Campos para email e senha.
- Botão de login.
- Link para registro caso o usuário não tenha uma conta.

### Tela Principal: Sistema de Gerenciamento de Tarefas
**Estrutura Geral:**

#### Cabeçalho (Header):
- Logo do sistema.
- Links de navegação (ex: Home, Tarefas).
- Botão de login/logout no canto superior direito.

#### Corpo Principal (Main Content):

##### Barra Lateral (Sidebar):
- Links de navegação para diferentes seções (ex: Todas as Tarefas, Tarefas Pendentes, Tarefas Concluídas).

##### Área de Conteúdo (Content Area):
**Lista de Tarefas:**
- Tabela ou cards exibindo as tarefas do usuário.
- Cada tarefa deve exibir o título, descrição (resumida), data de criação e status.
- Botões para editar e excluir cada tarefa.
- Botão para adicionar nova tarefa.

## Bibliotecas para Testes
Para a implementação dos testes unitários, escolha uma das seguintes bibliotecas e justifique sua escolha no README do projeto:
- Jest: Uma biblioteca de testes completa e muito popular no ecossistema JavaScript.
- React Testing Library: Focada em testes de componentes React, promovendo boas práticas de acessibilidade e testes mais próximos do uso real.
- Cypress: Excelente para testes end-to-end, com uma interface amigável e poderosa.
- Playwright: Uma biblioteca moderna para testes end-to-end, que suporta múltiplos navegadores e é altamente configurável.
- Enzyme: Outra biblioteca popular para testes de componentes React, especialmente útil para testes de shallow rendering.

## Critérios de Avaliação
**Funcionalidade:**
- Todas as funcionalidades descritas nos requisitos foram implementadas corretamente.
- As operações de CRUD estão funcionando conforme esperado.

**Autenticação e Segurança:**
- A autenticação via Auth0 está corretamente configurada e funcionando.
- As rotas protegidas estão realmente inacessíveis para usuários não autenticados.

**Código e Boas Práticas:**
- Código bem organizado, limpo e seguindo boas práticas de desenvolvimento.
- Uso adequado dos recursos do NextJS, react-hook-form, Tanstack Query e Tailwind CSS.
- Uso adequado do Prettier para formatação de código.
- Configuração de Husky para garantir qualidade antes dos commits.
- Documentação clara e abrangente.

**Teste e Manutenção:**
- Implementação de testes unitários utilizando a biblioteca escolhida.
- Justificativa clara para a escolha da biblioteca de testes no README.
- Facilidade para configurar e rodar o projeto localmente seguindo as instruções do README.

## Entrega
- O candidato deve fornecer um link para o repositório do GitHub contendo o código-fonte do projeto, juntamente com instruções claras no README sobre como configurar e executar o projeto localmente.
- O candidato deve fazer o deploy da aplicação utilizando Vercel e incluir o link para a aplicação funcionando no README.