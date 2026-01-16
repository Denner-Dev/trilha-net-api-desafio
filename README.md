# 🎯 Desafio Trilha .NET - API de Tarefas

Desafio de projeto da DIO Trilha .NET. Implementar uma API REST completa para gerenciamento de tarefas com endpoints CRUD.

## ✨ Funcionalidades

- ✅ Criar nova tarefa
- ✅ Ler/Listar tarefas
- ✅ Atualizar tarefa
- ✅ Deletar tarefa
- ✅ Integração com banco de dados
- ✅ Documentação com Swagger

## 🛠️ Tecnologias

- C# 11
- .NET 6+
- Entity Framework Core
- SQL Server / LocalDB
- Swagger/OpenAPI

## 🚀 Como Executar

### Pré-requisitos
- .NET 6 ou superior
- SQL Server ou LocalDB
- Visual Studio 2022 ou VS Code

### Instalação

```bash
git clone https://github.com/Denner-Dev/trilha-net-api-desafio.git
cd trilha-net-api-desafio
```

### Configurar Banco de Dados

1. Abra o arquivo `appsettings.json`
2. Configure a ConnectionString do seu SQL Server
3. Execute migrations:
   ```bash
   dotnet ef database update
   ```

### Executar

```bash
dotnet run
```

A API estará disponível em: `https://localhost:7000`
Swagger disponível em: `https://localhost:7000/swagger`

## 📚 Endpoints

| Método | Endpoint | Descrição |
|--------|----------|-----------|
| GET | `/api/tarefas` | Listar todas as tarefas |
| GET | `/api/tarefas/{id}` | Obter tarefa por ID |
| POST | `/api/tarefas` | Criar nova tarefa |
| PUT | `/api/tarefas/{id}` | Atualizar tarefa |
| DELETE | `/api/tarefas/{id}` | Deletar tarefa |

## 📋 Schema Tarefa

```json
{
  "id": 1,
  "titulo": "Minha Tarefa",
  "descricao": "Descrição da tarefa",
  "dataCriacao": "2024-01-16",
  "dataVencimento": "2024-01-20",
  "status": "Pendente"
}
```

## 📁 Estrutura

```
trilha-net-api-desafio/
├── Program.cs
├── appsettings.json
├── Controllers/
│   └── TarefasController.cs
├── Models/
│   └── Tarefa.cs
├── Context/
│   └── TarefasDbContext.cs
├── Migrations/
└── README.md
```

##  Licença

MIT
