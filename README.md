<p align="center">
  <img src="docs/images/capa-gauchao.png"
       alt="Álbum de Figurinhas do Gauchão"
       width="100%">
</p>

# ⚽ Álbum de Figurinhas Gauchão

<p align="center">
  Plataforma web para colecionar, organizar e acompanhar um álbum digital dos clubes participantes do Campeonato Gaúcho.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/status-em%20planejamento-F9A825" alt="Status do projeto">
  <img src="https://img.shields.io/badge/vers%C3%A3o-0.1.0-1976D2" alt="Versão">
  <img src="https://img.shields.io/badge/front--end-HTML%20%7C%20CSS%20%7C%20JavaScript-E34F26" alt="Front-end">
  <img src="https://img.shields.io/badge/back--end-PHP%20%7C%20Node.js-777BB4" alt="Back-end">
  <img src="https://img.shields.io/badge/banco-MySQL-4479A1" alt="Banco de dados">
</p>

---

## 📖 Sobre o projeto

O **Álbum de Figurinhas Gauchão** é uma plataforma digital criada para transformar a experiência tradicional de colecionar figurinhas em uma atividade organizada, interativa e acessível.

O sistema permitirá que cada usuário possua seu próprio álbum digital, consulte os clubes e jogadores participantes, registre as figurinhas conquistadas, identifique as faltantes e controle as repetidas disponíveis para futuras trocas.

Além da área destinada aos colecionadores, o projeto contará com um painel administrativo para gerenciamento de usuários, clubes, jogadores, temporadas, categorias e figurinhas.

---

## 🎯 Objetivo geral

Desenvolver uma plataforma web moderna, segura e responsiva para gerenciamento de um álbum digital de figurinhas relacionado ao Campeonato Gaúcho de Futebol.

---

## ✨ Principais funcionalidades

### Colecionador

- Cadastro e autenticação de usuário;
- Álbum individual por temporada;
- Visualização das figurinhas por clube;
- Registro de figurinhas conquistadas;
- Identificação das figurinhas faltantes;
- Controle da quantidade de repetidas;
- Percentual de conclusão do álbum;
- Progresso geral e por clube;
- Pesquisa por número, nome, clube ou categoria;
- Perfil e clube favorito;
- Sistema de trocas entre colecionadores;
- Notificações e histórico de atividades.

### Administrador

- Dashboard administrativo;
- Gerenciamento de usuários;
- Cadastro de temporadas;
- Cadastro de clubes e estádios;
- Cadastro de jogadores;
- Cadastro de categorias;
- Cadastro e numeração de figurinhas;
- Upload e gerenciamento de imagens;
- Relatórios e estatísticas;
- Controle de status e permissões;
- Registros de auditoria.

---

## 👥 Perfis de acesso

| Perfil | Responsabilidades |
|---|---|
| **Colecionador** | Gerenciar o próprio álbum, perfil, figurinhas e solicitações de troca |
| **Administrador** | Gerenciar todos os cadastros, usuários, temporadas, conteúdos e relatórios |
| **Moderador** | Perfil opcional para acompanhamento de conteúdos, denúncias e negociações |

---

## 🧩 Organização prevista do álbum

Cada clube poderá possuir inicialmente:

- 1 figurinha do escudo;
- 1 figurinha do uniforme;
- 1 figurinha do estádio;
- 1 figurinha do técnico;
- 13 figurinhas de jogadores principais;
- Figurinhas especiais e comemorativas.

O álbum também poderá incluir:

- Capa oficial;
- Apresentação da competição;
- Troféu;
- Estádios;
- Clubes participantes;
- Técnicos;
- Destaques;
- Figurinhas raras;
- Página de conclusão.

---

## 💻 Tecnologias planejadas

### Front-end

- HTML5;
- CSS3;
- JavaScript;
- Bootstrap ou Tailwind CSS;
- Fetch API ou Axios;
- Bibliotecas de ícones;
- Design responsivo.

### Back-end

- PHP 8 ou superior;
- Laravel;
- Composer;
- API REST;
- Laravel Sanctum ou JWT;
- Node.js;
- Express;
- Socket.IO.

### Banco de dados

- MySQL;
- MySQL Workbench;
- Migrations e seeders;
- Relacionamentos, índices e restrições;
- Backups periódicos.

### Ferramentas

- Git;
- GitHub;
- GitHub Wiki;
- Visual Studio Code;
- Figma;
- Postman;
- MySQL Workbench;
- XAMPP ou Laragon;
- Docker, opcionalmente.

---

## 🏗️ Arquitetura prevista

```text
Usuário
   │
   ▼
Interface Web
HTML + CSS + JavaScript
   │
   ▼
API REST
PHP / Laravel
   │
   ├── Serviço Node.js
   │   Notificações, chat e atualizações em tempo real
   │
   ▼
Banco de Dados
MySQL
```

A arquitetura será organizada em camadas:

- **Apresentação:** páginas, formulários, cards, tabelas e dashboards;
- **Aplicação:** controllers, rotas, autenticação e validações;
- **Negócio:** regras do álbum, progresso, repetidas e trocas;
- **Dados:** models, migrations, relacionamentos e consultas;
- **Tempo real:** notificações, chat e eventos utilizando Node.js.

---

## 📁 Estrutura de pastas planejada

```text
album-figurinhas-gauchao/
│
├── frontend/
│   ├── assets/
│   │   ├── css/
│   │   ├── js/
│   │   ├── images/
│   │   └── icons/
│   ├── components/
│   ├── pages/
│   └── index.html
│
├── backend/
│   ├── app/
│   │   ├── Controllers/
│   │   ├── Models/
│   │   ├── Services/
│   │   ├── Repositories/
│   │   └── Middleware/
│   ├── database/
│   │   ├── migrations/
│   │   └── seeders/
│   ├── routes/
│   ├── storage/
│   └── tests/
│
├── realtime-service/
│   ├── src/
│   │   ├── controllers/
│   │   ├── services/
│   │   ├── sockets/
│   │   └── routes/
│   ├── package.json
│   └── server.js
│
├── database/
│   ├── scripts/
│   ├── backups/
│   └── diagramas/
│
├── docs/
│   ├── requisitos/
│   ├── wireframes/
│   ├── diagramas/
│   └── imagens/
│
├── .gitignore
├── LICENSE
└── README.md
```

---

## 🗄️ Banco de dados

Entre as principais entidades previstas estão:

| Entidade | Finalidade |
|---|---|
| `usuarios` | Dados dos colecionadores e administradores |
| `perfis` | Perfis e permissões |
| `temporadas` | Edições do Campeonato Gaúcho |
| `clubes` | Clubes participantes |
| `estadios` | Estádios relacionados aos clubes |
| `jogadores` | Jogadores vinculados aos clubes e temporadas |
| `categorias` | Categorias das figurinhas |
| `figurinhas` | Figurinhas cadastradas |
| `albuns` | Álbum individual de cada usuário |
| `colecoes` | Figurinhas conquistadas e suas quantidades |
| `trocas` | Solicitações de troca |
| `itens_troca` | Figurinhas oferecidas e solicitadas |
| `notificacoes` | Avisos enviados aos usuários |
| `logs` | Histórico de ações importantes |

---

## 🔌 API

A API seguirá o padrão REST e utilizará respostas em JSON.

Exemplo de resposta:

```json
{
  "sucesso": true,
  "mensagem": "Operação realizada com sucesso.",
  "dados": {}
}
```

Principais grupos de endpoints:

```text
/api/auth
/api/usuarios
/api/temporadas
/api/clubes
/api/jogadores
/api/figurinhas
/api/albuns
/api/colecao
/api/trocas
/api/notificacoes
/api/admin
```

A documentação completa ficará disponível na [Wiki do projeto](../../wiki/API).

---

## 🚀 Instalação

> As instruções abaixo representam a estrutura planejada e poderão ser ajustadas durante o desenvolvimento.

### Pré-requisitos

- Git;
- PHP 8 ou superior;
- Composer;
- Node.js;
- npm;
- MySQL;
- Visual Studio Code;
- XAMPP ou Laragon, opcionalmente.

### 1. Clonar o repositório

```bash
git clone URL_DO_REPOSITORIO
cd album-figurinhas-gauchao
```

### 2. Configurar o back-end

```bash
cd backend
composer install
```

Crie o arquivo de ambiente:

```bash
cp .env.example .env
```

No Windows:

```bash
copy .env.example .env
```

Gere a chave da aplicação:

```bash
php artisan key:generate
```

### 3. Configurar o banco de dados

Crie o banco:

```sql
CREATE DATABASE album_gauchao
CHARACTER SET utf8mb4
COLLATE utf8mb4_unicode_ci;
```

Configure o arquivo `.env`:

```env
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=album_gauchao
DB_USERNAME=root
DB_PASSWORD=
```

Execute as migrations e os dados iniciais:

```bash
php artisan migrate --seed
```

### 4. Iniciar o back-end

```bash
php artisan serve
```

Endereço padrão:

```text
http://localhost:8000
```

### 5. Iniciar o serviço Node.js

```bash
cd realtime-service
npm install
npm run dev
```

### 6. Executar o front-end

Abra a pasta `frontend` com o **Live Server** ou execute o comando previsto no projeto.

```text
http://localhost:5500
```

Consulte as instruções detalhadas na [página de instalação](../../wiki/Instalação).

---

## 🔐 Variáveis de ambiente

Exemplo:

```env
APP_NAME="Album de Figurinhas Gauchao"
APP_ENV=local
APP_DEBUG=true
APP_URL=http://localhost:8000

DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=album_gauchao
DB_USERNAME=root
DB_PASSWORD=

FRONTEND_URL=http://localhost:5500
NODE_SERVICE_URL=http://localhost:3000
JWT_SECRET=chave_secreta
```

> Nunca envie o arquivo `.env` para o GitHub.

---

## 🎨 Identidade visual

A identidade visual será inspirada em:

- Futebol gaúcho;
- Colecionismo;
- Tecnologia;
- Competição;
- Comunidade;
- Tradição e modernidade.

Cores sugeridas:

| Cor | Código | Aplicação |
|---|---|---|
| Azul escuro | `#12355B` | Navegação e elementos institucionais |
| Azul médio | `#1976D2` | Botões e destaques |
| Verde | `#2E7D32` | Progresso e figurinhas conquistadas |
| Amarelo | `#F9A825` | Figurinhas especiais e alertas |
| Vermelho | `#C62828` | Erros e ações críticas |
| Grafite | `#20252B` | Textos e modo escuro |

---

## 📱 Responsividade

A plataforma será desenvolvida com abordagem **Mobile First**.

Quantidade estimada de figurinhas por linha:

| Dispositivo | Quantidade |
|---|---|
| Smartphone | 1 ou 2 |
| Tablet | 2 ou 3 |
| Notebook | 4 ou 5 |
| Desktop grande | 5 ou 6 |

A interface deverá possuir:

- Menu adaptável;
- Cards responsivos;
- Formulários em uma coluna no celular;
- Tabelas com adaptação ou rolagem;
- Imagens proporcionais;
- Botões adequados para toque;
- Modo claro e escuro.

---

## 🖼️ Wireframes

Os wireframes previstos incluem:

- Página inicial;
- Login e cadastro;
- Dashboard do colecionador;
- Álbum digital;
- Página de clubes;
- Cards das figurinhas;
- Figurinhas faltantes;
- Figurinhas repetidas;
- Sistema de trocas;
- Perfil;
- Dashboard administrativo;
- Cadastros administrativos;
- Versões desktop e mobile.

As imagens poderão ser armazenadas em:

```text
docs/wireframes/desktop/
docs/wireframes/mobile/
```

Consulte a [página de wireframes](../../wiki/Wireframes).

---

## 🗓️ Roadmap

### Concluído

- [x] Definição da ideia;
- [x] Levantamento inicial;
- [x] Definição dos perfis de acesso;
- [x] Estrutura inicial do álbum;
- [x] Definição das funcionalidades;
- [x] Criação dos wireframes iniciais;
- [x] Criação da documentação;
- [x] Criação da Wiki no GitHub.

### Em andamento

- [ ] Revisão do escopo da primeira versão;
- [ ] Identidade visual definitiva;
- [ ] Protótipo de alta fidelidade;
- [ ] Modelagem definitiva do banco de dados.

### Próximas etapas

- [ ] Configuração do projeto;
- [ ] Desenvolvimento da autenticação;
- [ ] Desenvolvimento dos cadastros;
- [ ] Implementação do álbum;
- [ ] Painel administrativo;
- [ ] Sistema de trocas;
- [ ] Testes;
- [ ] Publicação da versão 1.0.

Consulte o [roadmap completo](../../wiki/Roadmap).

---

## 🧪 Testes previstos

- Testes unitários;
- Testes de integração;
- Testes funcionais;
- Testes da API;
- Testes de segurança;
- Testes de responsividade;
- Testes de desempenho;
- Testes com usuários;
- Validação em diferentes navegadores.

---

## 📚 Documentação

A documentação completa está disponível na [Wiki do projeto](../../wiki).

Principais páginas:

- [Visão Geral](../../wiki/Visão-Geral);
- [Objetivos](../../wiki/Objetivos);
- [Funcionalidades](../../wiki/Funcionalidades);
- [Regras de Negócio](../../wiki/Regras-de-Negócio);
- [Tecnologias](../../wiki/Tecnologias);
- [Arquitetura do Sistema](../../wiki/Arquitetura-do-Sistema);
- [Banco de Dados](../../wiki/Banco-de-Dados);
- [API](../../wiki/API);
- [Instalação](../../wiki/Instalação);
- [Wireframes](../../wiki/Wireframes);
- [Identidade Visual](../../wiki/Identidade-Visual);
- [Responsividade](../../wiki/Responsividade);
- [Roadmap](../../wiki/Roadmap).

---


## 📄 Licença

A licença oficial do projeto ainda será definida.

Antes da utilização pública ou comercial de escudos, fotografias, uniformes e marcas dos clubes, será necessário verificar os direitos de uso e obter as autorizações necessárias.

---

## 👩‍💻 Autoria

**Mariana Bianchini Lima**  
Especialista em Tecnologia da Informação e Comunicação

---

<p align="center">
  Desenvolvido com dedicação para unir tecnologia, futebol gaúcho e colecionismo.
</p>
