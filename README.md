<h1>🍔 DevBurger API</h1>
Este repositório contém a API RESTful do projeto DevBurger, um sistema de gerenciamento de pedidos para lanchonetes, desenvolvido com foco em organização, segurança e escalabilidade. A API serve como base para o funcionamento da interface do cliente e do painel administrativo.

📌 Objetivo
O objetivo principal deste projeto é oferecer um backend robusto que permita o cadastro e autenticação de usuários, gerenciamento de produtos e pedidos, bem como o controle de fluxo dos pedidos (em preparo, pronto e entregue), integrando-se perfeitamente à interface desenvolvida em React.

🚀 Funcionalidades
Cadastro e autenticação de usuários (JWT)

Diferenciação entre usuários comuns e administradores

Cadastro, edição e exclusão de produtos (CRUD)

Upload de imagens com Multer

Cadastro e gerenciamento de pedidos

Atualização do status do pedido (em andamento → pronto → entregue)

Relacionamento entre usuários, pedidos e produtos

Validação de dados com Yup

🛠️ Tecnologias utilizadas
Node.js – Ambiente de execução JavaScript

Express.js – Framework para criação da API

PostgreSQL – Banco de dados relacional

Sequelize – ORM para facilitar a manipulação do banco

JWT – Autenticação segura com JSON Web Tokens

Multer – Upload de arquivos (imagens dos produtos)

Yup – Validação de dados

Cors & Dotenv – Suporte a ambiente e requisições externas

🗂️ Estrutura do projeto
A estrutura está dividida por responsabilidades, facilitando a manutenção e escalabilidade:

arduino
Copiar
Editar
src/
├── controllers/      → Lógica das rotas
├── middlewares/      → Autenticação, validações e tratamento de erros
├── models/           → Modelos do banco de dados com Sequelize
├── routes/           → Definição das rotas da API
├── services/         → Regras de negócio auxiliares
├── uploads/          → Armazenamento de imagens de produtos
├── validations/      → Esquemas de validação com Yup
🔧 Como executar localmente
Clone este repositório:

bash
Copiar
Editar
git clone https://github.com/Douglasl10/devburguer-api
Acesse a pasta do projeto:

bash
Copiar
Editar
cd devburguer-api
Instale as dependências:

bash
Copiar
Editar
npm install
Configure o arquivo .env com suas variáveis:

env
Copiar
Editar
DB_USER=seu_usuario
DB_PASS=sua_senha
DB_HOST=localhost
DB_NAME=devburger
JWT_SECRET=sua_chave_secreta
Execute as migrações e crie o banco:

bash
Copiar
Editar
npx sequelize db:create
npx sequelize db:migrate
Inicie o servidor:

bash
Copiar
Editar
npm start
A API estará disponível em http://localhost:3001

🌐 Integração com o Front-end
Este projeto foi desenvolvido para funcionar com a DevBurger Interface. Juntas, essas aplicações simulam um sistema completo de pedidos para lanchonetes.

<img src="https://raw.githubusercontent.com/Douglasl10/devburger-interface/refs/heads/main/img/DevBurger-Cadastro.png"/>
