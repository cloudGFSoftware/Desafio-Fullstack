# Desafio Técnico Full Stack – GF Software

Bem-vindo(a) ao desafio técnico para a vaga de Desenvolvedor Full Stack PLENO na GF Software! Este repositório contém as instruções para criar dois ambientes separados: um backend e um frontend.

---

## Desafio

Você deverá criar uma aplicação com dois ambientes:

1. **Backend:**  
   - **Tecnologias:** Node.js, Express, TypeScript.  
   - **Banco de Dados:** MongoDB utilizando Mongoose.  
   - **Funcionalidades:**  
     - CRUD de Usuários e Produtos.  
     - Autenticação utilizando token JWT.  
     - Controle de acesso com duas roles: **admin** e **cliente**.
       - **Admin:** Pode criar, visualizar, editar e excluir produtos.
       - **Cliente:** Pode apenas visualizar produtos.

2. **Frontend:**  
   - **Tecnologias:** Vite.js, React, TypeScript.  
   - **Funcionalidades:**  
     - Tela de Login.
     - Tela para visualização dos produtos com base na permissão do usuário:
       - Usuários **admin** devem ter acesso às opções para criar, editar ou excluir produtos.
       - Usuários **cliente** apenas visualizar os produtos.

---

## Requisitos do Desafio

### Backend

- **Endpoints para Usuários:**
  - Cadastro de usuários, definindo a role (admin/cliente).
  - Login com geração de token JWT.
  - Validação de token para acesso aos endpoints protegidos.
  - Entidade: 
    - Nome
    - Email
    - Senha
    - Permissão/Cargo

- **Endpoints para Produtos:**
  - CRUD completo para produtos.
  - Restrições de acesso:
    - Apenas usuários **admin** podem criar, editar e excluir produtos.
    - Todos os usuários autenticados podem visualizar os produtos.
  - Entidade: 
    - Nome
    - Descrição
    - Valor

- **Tecnologias e Ferramentas:**
  - Node.js com Express.
  - TypeScript.
  - MongoDB/Mongoose.
  - JWT para autenticação.

- **Dicas:**
  - Organize seu código em camadas (rotas, controllers, models, middlewares, etc.).
  - Adicione testes (mesmo que simples) para demonstrar a qualidade do código.
  - Documente suas rotas e a estrutura da API utilizando ferramentas como Swagger ou similar (opcional).

### Frontend

- **Tela de Login:**
  - Formulário para entrada de email/senha.
  - Integração com o backend para autenticação e obtenção do token JWT.

- **Tela de Produtos:**
  - Exibirá a lista de produtos retornados pela API.
  - Com base no perfil do usuário (admin/cliente), exibir ou ocultar os botões de:
    - Criar Produto.
    - Editar Produto.
    - Excluir Produto.

- **Tecnologias e Ferramentas:**
  - Vite.js com React.
  - TypeScript.
  - Bibliotecas opcionais de UI (ex: Material-UI, Bootstrap, etc.) conforme sua preferência.
  - Gerenciamento de estado (Context API, Redux, etc.) de forma opcional.

---

## Avaliação

Serão analisados os seguintes pontos:

- **Estrutura do Código:** Organização dos arquivos, modularização e boas práticas.
- **Funcionalidades:** Correta implementação das funcionalidades descritas, validação e controle de acesso.
- **Documentação:** Clareza nas instruções de setup, uso do README e comentários no código quando necessário.
- **Commits:** Uso de commits com descrições claras e consistentes demonstrando o progresso e a evolução do desenvolvimento.

---

# Entrega e Próximos Passos

## Entrega

- Faça um fork do repositório no GitHub e envie o link para análise.
- Certifique-se de que os commits demonstrem evolução e boas práticas.
- No README do seu repositório, inclua instruções claras para setup e execução dos projetos (backend e frontend).

---

## Conclusão e Próximos Passos

Após a submissão do desafio, daremos continuidade ao processo da seguinte maneira:

1. Revisão do código, funcionalidades, documentação e commits.
2. Entrevista técnica e/ou live coding (Fase 2).
3. Entrevista final para alinhamento e cultura (Fase 3).

Você receberá um retorno com nossa decisão e os próximos passos em até 1 semana.

---

Boa sorte e mãos à obra! Se tiver qualquer dúvida durante o desafio, sinta-se à vontade para entrar em contato.
