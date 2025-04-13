# 📝 CMS API – Sistema de Gerenciamento de Conteúdo

## 📖 Descrição
Esta API oferece um backend robusto para gerenciamento de conteúdo em aplicações web, construída com Next.js API Routes e TypeScript. Ideal para blogs, portfólios, landing pages ou qualquer aplicação que necessite de criação e organização de conteúdo dinâmico de forma centralizada e escalável.

## 🚀 Funcionalidades
 * 📄 Gerenciamento de Conteúdos (posts, páginas, artigos)

 * 🏷️ Categorias e Tags

 * 👤 Autenticação e Autorização

 * 📝 Editor-friendly (para integração com frontends headless)

 * 🧩 Estrutura modular e extensível

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
