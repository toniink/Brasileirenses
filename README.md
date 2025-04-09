
# 🇧🇷 Brasileirenses API

API desenvolvida para estudo e prática de criação de servidores com Node.js, Express e integração com banco de dados MySQL. Permite operações completas com a tabela de usuários.

---

## 🚀 Tecnologias Utilizadas

- **Node.js** – Ambiente de execução JavaScript
- **Express** – Framework para criação de APIs
- **MySQL** – Banco de dados relacional
- **dotenv** – Gerenciamento de variáveis de ambiente
- **nodemon** – Ferramenta para desenvolvimento com reinicialização automática

---

## 📦 Instalação

### 1. Clone o repositório

```bash
git clone https://github.com/toniink/brasileirenses
```

### 2. Acesse a pasta do projeto

```bash
cd brasileirenses
```

### 3. Instale as dependências

```bash
npm install
```

### 4. Configure o arquivo `.env`

Crie um arquivo `.env` na raiz do projeto e preencha com suas credenciais do MySQL:

```env
DB_HOST=localhost
DB_USER=root
DB_PASSWORD=suaSenhaAqui
DB_NAME=nomeDoBanco
# DB_PORT=3306 (opcional)
```

### 5. Inicie o servidor

```bash
npm run dev
```

Se tudo estiver certo, a saída será:

```
Servidor rodando na porta 3000
```

---

## 🧱 Estrutura do Projeto

```
brasileirenses/
│
├── node_modules/
├── src/
│   ├── controllers/
│   ├── routes/
│   ├── models/
│   └── server.js
│
├── .env
├── package.json
├── README.md
```

---

## 🗃️ Banco de Dados

- **Nome do banco:** `nomeDoBanco`
- **Tabela principal:** `usuarios`

### Estrutura da tabela `usuarios`:

| Campo         | Tipo         | Descrição                          |
|---------------|--------------|------------------------------------|
| `id`          | INT          | Chave primária (auto incremento)  |
| `nome`        | VARCHAR      | Nome do usuário                   |
| `email`       | VARCHAR      | Email do usuário                  |
| `senha`       | VARCHAR      | Senha do usuário (criptografada)  |
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

## 🧪 Testando com Thunder Client

1. Instale a extensão **Thunder Client** no VSCode.
2. Crie uma nova requisição.
3. Use os métodos **GET**, **POST**, **PUT** e **DELETE** com a URL:

```http
http://localhost:3000/usuarios
```

### Exemplo de corpo para POST ou PUT (JSON):

```json
{
  "nome": "Exemplo da Silva",
  "email": "exemplo@email.com",
  "senha": "123456"
}
```

---

## 👩‍💻 Desenvolvido por

**Marcelle**  
Estudante de Análise e Desenvolvimento de Sistemas  
Em busca de crescimento na área de programação 🚀
