# 📝 CMS API – Sistema de Gerenciamento de Conteúdo

## 📖 Descrição
Esta API oferece um backend robusto para gerenciamento de conteúdo em aplicações web, construída com Next.js API Routes e TypeScript. Ideal para blogs, portfólios, landing pages ou qualquer aplicação que necessite de criação e organização de conteúdo dinâmico de forma centralizada e escalável.

## 🚀 Funcionalidades
 * 📄 Gerenciamento de Conteúdos (posts, páginas, artigos)

 * 🏷️ Categorias e Tags

 * 👤 Autenticação e Autorização

 * 📝 Editor-friendly (para integração com frontends headless)

 * 🧩 Estrutura modular e extensível

## 🚀 Endpoints

### Conteúdos (Posts/Páginas)

| Método   | Endpoint           | Descrição                                                 |
|----------|--------------------|-----------------------------------------------------------|
| `GET`    | `/api/posts`       | Listar todos os conteúdos                                 |
| `GET`    | `/api/posts/:id`   | Obter detalhes de um conteúdo                             |
| `POST`   | `/api/posts`       | Criar novo conteúdo                                       |
| `PUT`    | `/api/posts/:id`   | Atualizar um conteúdo existente                           |
| `DELETE` | `/api/posts/:id`   | Remover um conteúdo                                       |

### Categorias

| Método   | Endpoint               | Descrição                              |
|----------|------------------------|----------------------------------------|
| `GET`    | `/api/categories`      | Listar todas as categorias             |
| `POST`   | `/api/categories`      | Criar uma nova categoria               |
| `PUT`    | `/api/categories/:id`  | Atualizar uma categoria existente      |
| `DELETE` | `/api/categories/:id`  | Remover uma categoria                  |

### Autenticação

| Método   | Endpoint               | Descrição                              |
|----------|------------------------|----------------------------------------|
| `POST`   | `/api/auth/login`      | Login e geração de token JWT           |
| `POST`   | `/api/auth/register`   | Registro de novo usuário               |
| `GET`    | `/api/auth/me`         | Obter dados do usuário autenticado     |


## 🛠️ Tecnologias Utilizadas
 * Next.js (API Routes)

 * TypeScript

 * Prisma ORM

 * SQLite (ou PostgreSQL, MySQL, adaptável)

 * Zod (validação)

 * JWT (autenticação)

 * Docker (opcional)

## ⚙️ Como Rodar Localmente
✅ Pré-requisitos
 * Node.js v20+

 * SQLite (ou outro banco configurado no Prisma)

 * Docker (opcional)

📦 Passo a Passo
  1. Clone o repositório
     ```Bash
     git clone https://github.com/seu-usuario/cms-api.git
     cd cms-api
     ```

  2. Configure o ambiente Crie um .env com:
     ```env
     DATABASE_URL="file:./dev.db"
     JWT_SECRET="sua-chave-secreta"
     ```
  
  3. Instale as dependências
     ```Bash
     npm install
     ```

  4. Configure o banco de dados
     ```Bash
     npx prisma migrate dev
     ```

  5. Execute o servidor
     ```Bash
     npm run dev
     ```
## 📁 Estrutura do Projeto (sugestiva)
```Bash
/
├── pages/
│   └── api/
│       ├── posts/
│       ├── categories/
│       └── auth/
├── prisma/
│   ├── schema.prisma
├── lib/
│   ├── auth.ts
│   ├── db.ts
│   └── validators.ts
├── middleware/
├── .env
├── Dockerfile
└── README.md
```

# 🔐 Segurança
  * JWT para autenticação de rotas protegidas

  * Middleware para verificação de token e permissões

  * Validações com Zod para todos os inputs

# 📦 Possíveis Extensões
  * Upload de imagens (via S3, Cloudinary, etc)

  * Painel administrativo (Next.js Admin UI)

  * Webhooks para publicação em produção

  * Suporte multilíngue


