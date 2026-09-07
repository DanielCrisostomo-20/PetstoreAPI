# 🐾 PetstoreAPI — Coleção Postman

Coleção de requisições HTTP para a [Petstore API](https://petstore.swagger.io/), uma API pública de exemplo para testes e aprendizado. Criada e organizada com o **Postman** em modo local (workspace filesystem).

---

## 📁 Estrutura da Coleção

```
New Collection/
└── PET/
    ├── POST   /v2/pet                                     → Adicionar novo pet
    ├── GET    /v2/pet/findByStatus?status=available       → Buscar pets por status
    ├── DELETE /v2/pet/2                                   → Deletar pet por ID
    └── STORE/
        ├── GET /v2/store/inventory                        → Ver inventário da loja
        ├── GET /v2/store/order/4                          → Buscar pedido por ID
        └── USER/
            └── POST /v2/user/createWithList               → Criar usuários em lista
```

---

## 🚀 Como usar

### Pré-requisitos
- [Postman](https://www.postman.com/downloads/) instalado
- Git instalado

### Clonar o repositório
```bash
git clone https://github.com/DanielCrisostomo-20/PetstoreAPI.git
```

### Abrir no Postman
1. Abra o Postman
2. Vá em **File > Open Workspace from Folder**
3. Selecione a pasta clonada
4. As coleções aparecerão automaticamente na sidebar

---

## 📋 Endpoints

### 🐶 PET

| Método | Endpoint | Descrição |
|--------|----------|-----------|
| `POST` | `/v2/pet` | Adiciona um novo pet à loja |
| `GET` | `/v2/pet/findByStatus?status=available` | Busca pets pelo status |
| `DELETE` | `/v2/pet/2` | Remove um pet pelo ID |

**Exemplo de body — POST /v2/pet:**
```json
{
  "id": 0,
  "category": { "id": 0, "name": "string" },
  "name": "doggie",
  "photoUrls": ["string"],
  "tags": [{ "id": 0, "name": "string" }],
  "status": "available"
}
```

---

### 🏪 STORE

| Método | Endpoint | Descrição |
|--------|----------|-----------|
| `GET` | `/v2/store/inventory` | Retorna o inventário da loja |
| `GET` | `/v2/store/order/4` | Busca um pedido pelo ID |

---

### 👤 USER

| Método | Endpoint | Descrição |
|--------|----------|-----------|
| `POST` | `/v2/user/createWithList` | Cria múltiplos usuários de uma vez |

**Exemplo de body — POST /v2/user/createWithList:**
```json
[
  {
    "id": 0,
    "username": "string",
    "firstName": "string",
    "lastName": "string",
    "email": "string",
    "password": "string",
    "phone": "string",
    "userStatus": 0
  }
]
```

---

## 🌐 Base URL

```
https://petstore.swagger.io/v2
```

---

## 🛠️ Tecnologias

- [Postman](https://www.postman.com/) — criação e organização das requisições
- [Petstore API](https://petstore.swagger.io/) — API pública de exemplo (Swagger)
- Git + GitHub — versionamento

---

## 👤 Autor

**Daniel Crisostomo**  
GitHub: [@DanielCrisostomo-20](https://github.com/DanielCrisostomo-20)
