# 🗄️ Projeto ORM com Prisma e TypeScript

Este repositório contém um projeto de estudo focado na implementação de um Object-Relational Mapper (ORM) utilizando Prisma e TypeScript, explorando a interação com banco de dados de forma eficiente e segura.

## ✨ Visão Geral

Este projeto foi desenvolvido para aprofundar o conhecimento em ORMs e na utilização do Prisma em conjunto com TypeScript. Ele demonstra como configurar um ambiente de desenvolvimento com tipagem forte, realizar operações CRUD (Create, Read, Update, Delete) em um banco de dados, gerenciar migrações e seeds, e garantir a consistência dos dados. O foco é na construção de uma camada de acesso a dados robusta e de fácil manutenção.

## 🛠️ Tecnologias Utilizadas

[![My Skills](https://skillicons.dev/icons?i=ts,nodejs,prisma,postgresql )](https://skillicons.dev )

-   **TypeScript**: Linguagem de programação que adiciona tipagem estática ao JavaScript, proporcionando maior segurança e consistência ao código.
-   **Node.js**: Ambiente de execução JavaScript server-side.
-   **Prisma**: ORM moderno e de próxima geração que simplifica o acesso ao banco de dados com um gerador de clientes TypeScript-first.
-   **PostgreSQL (ou SQLite)**: Banco de dados relacional utilizado para persistir os dados da aplicação. (Ajustar conforme o banco de dados real utilizado, o `package.json` sugere `sqlite` para desenvolvimento).

## 🚀 Como Usar

Para configurar e executar o projeto localmente, siga os passos abaixo:

1.  **Clone o repositório:**
    ```bash
    git clone https://github.com/FelipeFerreiraAmado/ORM.git
    ```
2.  **Navegue até o diretório do projeto:**
    ```bash
    cd ORM
    ```
3.  **Instale as dependências:**
    ```bash
    npm install
    ```
4.  **Configure o banco de dados:**
    -   Crie um arquivo `.env` na raiz do projeto com a string de conexão do seu banco de dados. Exemplo para SQLite:
        ```
        DATABASE_URL="file:./dev.db"
        ```
        Ou para PostgreSQL:
        ```
        DATABASE_URL="postgresql://user:password@localhost:5432/database_name?schema=public"
        ```
5.  **Execute as migrações do Prisma para criar o esquema do banco de dados:**
    ```bash
    npx prisma migrate dev --name init
    ```
6.  **Gere o cliente Prisma:**
    ```bash
    npx prisma generate
    ```
7.  **Execute os seeds (se houver ) para popular o banco de dados com dados iniciais:**
    ```bash
    npx prisma db seed
    ```
8.  **Inicie a aplicação (se houver um script de inicialização, como um servidor):**
    ```bash
    npm run dev # ou o comando apropriado para iniciar sua aplicação
    ```

## 💡 Funcionalidades e Destaques

-   **Modelagem de Dados**: Definição de modelos de dados com o Schema do Prisma.
-   **Operações CRUD**: Implementação de funcionalidades para Criar, Ler, Atualizar e Deletar registros no banco de dados.
-   **Migrações de Banco de Dados**: Gerenciamento de alterações no esquema do banco de dados com o Prisma Migrate.
-   **Seeds de Dados**: População inicial do banco de dados com dados de exemplo.
-   **Tipagem Segura**: Benefícios do TypeScript para garantir a segurança dos tipos em todas as interações com o banco de dados.

## 🔮 Melhorias Futuras

-   Implementar autenticação e autorização.
-   Adicionar mais modelos de dados e relacionamentos complexos.
-   Integrar com uma API RESTful completa ou um framework web (e.g., Express, NestJS).
-   Testes unitários e de integração.
-   Documentação da API com Swagger/OpenAPI (se integrada a uma API).

## 🤝 Contribuição

Contribuições são sempre bem-vindas! Se você tem ideias para melhorar este projeto, sinta-se à vontade para:

1.  Fazer um fork do repositório.
2.  Criar uma nova branch (`git checkout -b feature/sua-feature`).
3.  Fazer suas alterações e commit (`git commit -m \'Adiciona nova feature\'`).
4.  Enviar para a branch (`git push origin feature/sua-feature`).
5.  Abrir um Pull Request.

## 📄 Licença

Este projeto está licenciado sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.
