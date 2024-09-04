# bondy-desafio-fullstack

## Estrutura do Repositório

- **backend**: API GraphQL para realizar o desafio de backend
- **frontend**: Repositório para criação do frontend do desafio

## Instruções de Execução

Para executar os scripts presentes nos arquivos `package.json`:

- Para executar um comando em todos os pacotes: `yarn lerna run <comando>` (exemplo: `yarn lerna run test:coverage`)
- Para executar um comando em um pacote específico: `yarn lerna run <comando> --scope=<nome-do-pacote>` (exemplo: `yarn lerna run start --scope=backend`)
- Para executar comandos diretamente no pacote específico: Entre na pasta do pacote e execute o comando normalmente.

## Backend

### Funcionalidades Implementadas

- **Mutation de Login**: Foi criada uma mutation para realizar o login. Ela recebe e-mail e senha e faz a verificação no banco de dados. A mutation retorna todas as informações salvas no modelo `User`.
- **Mutation de Register**: Foi criada uma mutation para realizar o Registro. Ela recebe e-mail, senha e nome e faz a verificação no banco de dados. A mutation retorna todas as informações salvas no modelo `User`.

### Como Executar

1. Navegue até a pasta `backend`.
2. Instale as dependências.
3. Inicie o servidor.
4. Acesse o Playground GraphQL na URL exibida no console para testar a mutation de login.

## Frontend

### Configuração

- Instalar Dependências: Entre na pasta `packages/frontend` e execute `yarn` para instalar as dependências do frontend.

### Tecnologias Utilizadas

- **Framework**: Next.js
- **Estilização**: TailwindCSS
- **Component Library**: Radix UI
- **Validação**: Zod
- **GraphQL**: Utilizado para comunicação com o backend

### Funcionalidades Implementadas

- **Página de Login**: Permite ao usuário inserir e-mail e senha. Realiza uma consulta GraphQL para autenticação e, se as credenciais estiverem corretas, redireciona para a página de boas-vindas.
- **Página de Registro**: Permite o registro de novos usuários. Realiza uma consulta GraphQL para criar um novo usuário no backend.
- **Página de Agradecimento**: Exibe uma mensagem de boas-vindas após o login bem-sucedido.

### Execução

Para iniciar o frontend, entre na pasta `packages/frontend` e execute `yarn run dev`. O aplicativo estará disponível em `http://localhost:4000`.
