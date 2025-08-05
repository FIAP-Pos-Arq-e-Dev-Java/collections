# 🧪 Collection de Testes - Microsserviços de Login e Usuário

Este repositório contém uma coleção de testes Postman estruturada para validar os microsserviços `ms-login` e `ms-usuario`. A collection cobre todos os fluxos principais das aplicações, tanto de sucesso quanto de erro.

---

## 📁 Estrutura da Collection

A collection está dividida em três grandes pastas:

### 1. **ms-login**
Contém chamadas para o microsserviço de login de uma forma geral.

### 2. **ms-restaurante**
Contém chamadas para o microsserviço de usuários de uma forma geral.

### 3. **Cenários de Testes Manuais**
Pasta com **testes manuais** divididos em subpastas, separando os cenários de **sucesso e erro** por funcionalidade, como:

- `Gerencimento de restaurantes`
- `Gerencimento de itens de cardápio`
- `Gerencimento de tipos de cozinha` 
- `Gerencimento de usuários`
- `Gerenciamento de geração de token Oauth`
---

## 🌐 Arquivo de Ambiente

A collection utiliza um arquivo `.postman_environment.json` com as seguintes variáveis:

| Serviço     | Porta | URL Base                         |
|-------------|-------|----------------------------------|
| ms-login    | 9207  | `http://localhost:8080/` |
| ms-restaurante  | 9808  | `http://localhost:8081/ms-restaurante` |

Essas variáveis facilitam a execução dos testes sem precisar alterar manualmente os endpoints.

---

## ▶️ Como Executar os Testes no Postman

1. **Importe** a collection (`.postman_collection.json`) no Postman.
2. **Importe** o ambiente (`.postman_environment.json`).
3. Navegue até as pastas e **execute os testes** manualmente.

---

## ✅ Requisitos para os testes passarem

- Microsserviços ms-login e ms-restaurante devem estar executando localmente nas portas 8080 e 8081, respectivamente.
 
- Banco de dados deve estar disponível e corretamente populado, conforme os cenários esperados.


