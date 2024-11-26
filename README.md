# Site Uniesp 2024

Este é um projeto desenvolvido para a disciplina de Tecnoligia para Front-End Avançado da UNIESP. 

---
- Bibliotecas Utilizadas:
  
 - React: Estrutura os componentes(Navbar e os formulários) e gerencia os estados e efeitos da aplicação.
 - React Router Dom: Gerencia as rotas e navegação entre páginas pelo ID como inicial, notícias e contato.
 - Axios: Realiza requisições HTTP. Comunicação com o backend falso (json-server), para buscar, cadastrar, editar e deletar notícias.
 - Material-UI (MUI): Fornece componentes prontos e estilizados, como botões e campos de texto.
 - JSON-Server: Simula um backend RESTful para armazenar e manipular dados das notícias.
 - Vite: Configura o ambiente de desenvolvimento e build rápido.


-Funcionalidades do Projeto:

  -Cadastro de Notícias:
   - Permite adicionar notícias com título, subtítulo e texto.
   - Dados armazenados localmente utilizando o **json-server**.

  -Listagem de Notícias:
   - Exibe todas as notícias cadastradas em uma interface amigável.
   - Cada item possui opções para edição e exclusão.

  -Edição de Notícias:
   - Permite alterar o título, subtítulo e texto das notícias cadastradas.

  -Exclusão de Notícias:
   - Remove notícias do sistema permanentemente.

---

## Estrutura do Projeto


```plaintext
.
├── data/
│   ├── db.json                # Estrutura do Banco de Dados. Utilizado pelo json-server.
├── public/
├── src/
│   ├── components/            # Componentes reutilizáveis no projeto
│   │   ├── BannerAd.jsx       # Utilizado para propagandas ou informativos.
│   │   ├── NavBar.jsx         # Usado para navegação entre páginas.
│   ├── pages/                 # Página principais do site
│   │   ├── admin/
│   │   │   ├── AdminNoticias.jsx   # Página de administração das notícias.
│   │   │   ├── CadastroNoticia.jsx # Página para cadastrar notícias.
│   │   │   ├── EditarNoticia.jsx   # Página para editar notícias.
│   │   ├── Contato.jsx             # Página de contato com a Instituição.
│   │   ├── DpoLgpd.jsx             # Página com informações sobre LGPD.
│   │   ├── Faculdade.jsx           # Página com informações gerais sobre a instituição.
│   │   ├── Inicial.jsx             # Página inicial com informações básicas da Instituição.
│   │   ├── Noticias.jsx            # Página de notícias da instituição.
│   │   ├── VisualizaNoticia.jsx    # responsável por exibir os detalhes de uma notícia específica. Ele utiliza o React Router para indentificar o ID e faz uma requisição na API para pegar os dados. 
│   │   │                           # Utiliza React Router para identificar o ID e fazer requisição na API.
│   ├── App.jsx                 # Arquivo principal que gerencia as rotas.
│   ├── index.jsx               # Ponto de entrada do React.
├── package.json                # Arquivo de configuração do projeto.
└── README.md                   # Documentação do projeto.

