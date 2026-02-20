# Documento de Requisitos

## 1. Requisitos Funcionais

### RF01 - Cadastro de Usuário
O sistema deve permitir que o usuário realize cadastro informando nome, e-mail e senha.

**Critérios de Aceitação:**
- Todos os campos são obrigatórios.
- O e-mail deve ser válido.
- Não permitir e-mail já cadastrado.

---

### RF02 - Login de Usuário
O sistema deve permitir que o usuário realize login.

**Critérios de Aceitação:**
- Deve validar e-mail e senha.
- Exibir mensagem de erro se inválido.
- Criar sessão se válido.

---

### RF03 - Cadastro de Produto
O sistema deve permitir cadastrar produtos.

**Critérios de Aceitação:**
- Nome, descrição e preço são obrigatórios.
- Preço deve ser maior que zero.

---

### RF04 - Listagem de Produtos
O sistema deve exibir todos os produtos cadastrados.

**Critérios de Aceitação:**
- Mostrar nome, descrição e preço.
- Atualizar lista após novo cadastro.

---

## 2. Requisitos Não Funcionais

### RNF01 - Desempenho
O sistema deve responder em até 2 segundos.

**Critérios de Verificação:**
- Testes devem comprovar tempo máximo de 2 segundos.

---

### RNF02 - Segurança
As senhas devem ser armazenadas criptografadas.

**Critérios de Verificação:**
- Senhas não podem estar em texto puro no banco.

---

## 3. Regras de Negócio

### RN01 - E-mail Único
Não é permitido dois usuários com o mesmo e-mail.

**Critério de Verificação:**
- Sistema deve bloquear cadastro duplicado.

---

### RN02 - Preço Positivo
Produto deve ter preço maior que zero.

**Critério de Verificação:**
- Sistema deve impedir preço ≤ 0.
