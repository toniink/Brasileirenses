# Brasileirenses API
API desenvolvida para estudo e prática de criação de servidores com Node.js, Express e integração com banco de dados SQLite. Permite operações completas com a tabela de usuários.

---

## 🚀 Tecnologias Utilizadas
- **Node.js** – Ambiente de execução JavaScript

- **Express** – Framework para criação de APIs

- **SQLite** – Banco de dados leve e relacional

- **Git** – Controle de versão

---

## 📦 Instalação
### 1. Clone o repositório

```bash
git clone https://github.com/toniink/brasileirenses
```

### 2. Acesse a pasta do projeto
```
bash
cd brasileirenses
```

### 3. Instale as dependências

```
bash
npm install
```

### 4. Inicie o servidor
Execute o comando para iniciar o servidor:
```
bash
node server.js
```
Se tudo estiver certo, a saída será:

```
bash
Servidor rodando na porta 3000
```

Para acessar a interface web, abra o arquivo public/index.html diretamente no navegador.

---

## 🧱 Estrutura do Projeto

```
brasileirenses/
│
├── config/
│   └── db.js            # Configuração do banco SQLite
│
├── node_modules/        # Dependências instaladas
├── public/
│   ├── index.html       # Página inicial
│   ├── styles.css       # Estilos da interface
│   ├── script.js        # Lógica da interface
│
├── .gitignore           # Arquivos ignorados pelo Git
├── database.db          # Banco de dados SQLite
├── package-lock.json    # Informações de dependências instaladas
├── package.json         # Configurações do projeto
├── README.md            # Documentação do projeto
└── server.js            # Servidor com Node.js e Express
```
---

### 🗃️ Banco de Dados
- **Nome do banco**: `database.db`

- **Tabela principal**: `usuarios`

### Estrutura da tabela `usuarios`:
| Campo         | Tipo         | Descrição                          |
|---------------|--------------|------------------------------------|
| `id`          | INTEGER      | Chave primária (auto incremento)  |
| `nome`        | TEXT         | Nome do usuário                   |
| `email`       | TEXT         | Email do usuário                  |
| `senha`       | TEXT         | Senha do usuário (criptografada)  |
| `data_criacao`| DATETIME     | Data de criação do registro       |

---

## 🔄 Endpoints da API

| Método | Rota                       | Descrição                          |
|--------|----------------------------|------------------------------------|
| GET    | `/usuarios`                | Lista todos os usuários            |
| GET    | `/usuarios/:id`            | Retorna um usuário específico      |
| POST   | `/usuarios`                | Cria um novo usuário               |
| PUT    | `/usuarios/:id`            | Atualiza um usuário existente      |
| DELETE | `/usuarios/:id`            | Remove um usuário pelo ID          |

---

## 🧪 Inicialização e Teste
Para inicializar o projeto e acessar a interface web, abra diretamente o arquivo public/index.html no navegador.

Teste a API diretamente no navegador ou use formulários da página web (index.html) para interagir com o backend.

👩‍💻 Desenvolvido por:  
Antonio Tavares  
Estefane Rodrigues   
Graziely Vargas  
Lidia Pereira  
Marcele Rodrigues  
