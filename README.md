# Sobre o projeto

**Descrição do Projeto:**

Este projeto consiste em uma aplicação web desenvolvida com **React** no front-end e **Firebase** no back-end, focada em fornecer uma experiência fluida e segura para os usuários, além de uma interface de administração eficiente. 

### Principais funcionalidades:
- **Autenticação de Usuários**: Utilizei o Firebase Authentication para implementar o login e o registro de usuários, com suporte a diferentes métodos de autenticação, como email/senha e provedores externos.
  
- **Gerenciamento de Rotas com Redirects**: A navegação pela aplicação foi estruturada com **React Router**, garantindo a proteção de rotas com base na autenticação. Usuários não autenticados são redirecionados automaticamente para a página de login.

- **Consumo da API do Firebase**: A aplicação interage com o Firebase Firestore para realizar operações de CRUD (Create, Read, Update e Delete) de forma eficiente. Isso permite o gerenciamento dinâmico de posts pelos usuários autenticados.

- **CRUD de Posts**: Implementação completa de CRUD de posts, onde os usuários podem criar, visualizar, editar e excluir postagens. Cada post é armazenado no Firestore, e a interface foi projetada para ser intuitiva e responsiva.

- **Dashboard**: Um dashboard foi desenvolvido para permitir que os administradores ou usuários autenticados visualizem suas postagens e tenham acesso a funcionalidades de gestão de de posts

### Outros Recursos:
- **Redirecionamento Condicional**: Com base no estado de autenticação do usuário, a aplicação redireciona automaticamente para a página correta.
- **Componentização e Reutilização de Código**: O código foi modularizado para garantir facilidade de manutenção e reutilização de componentes React.
- **Responsividade**: O layout foi desenvolvido com atenção à responsividade, garantindo uma boa experiência tanto em dispositivos móveis quanto em desktop.

## Inicialização do Projeto

### Passo 1: Configuração do Firebase
1. Acesse o [Firebase Console](https://console.firebase.google.com/), crie um novo projeto e configure os serviços necessários (Firestore, Authentication, etc.).
2. Após a criação do projeto, obtenha as credenciais de configuração (API Key, Auth Domain, Project ID, etc.) que serão utilizadas para conectar sua aplicação ao Firebase.

### Passo 2: Configuração do Ambiente
1. No diretório raiz do seu projeto, renomeie o arquivo `.env-example` para `.env`.
2. Insira as variáveis de ambiente do Firebase que você obteve na etapa anterior no arquivo `.env`:
   ```bash
    REACT_APP_API_KEY=your-api-key
    REACT_APP_AUTH_DOMAIN= your-auth-domain
    REACT_APP_PROJECT_ID=your-project-id
    REACT_APP_STORAGE_BUCKET=your-storage-bucket
    REACT_APP_MESSAGING_SENDER_ID=your-messaging-sender-id
    REACT_APP_APP_ID==your-app-id
   ```

### Passo 3: Iniciando o Projeto
1. No diretório do projeto, abra o terminal e execute o seguinte comando para instalar as dependências:
   ```bash
   npm install
   ```
2. Após a instalação das dependências, inicie o servidor de desenvolvimento com o comando:
   ```bash
   npm start
   ```
3. O projeto será iniciado e estará acessível no navegador através do endereço `http://localhost:3000`.
