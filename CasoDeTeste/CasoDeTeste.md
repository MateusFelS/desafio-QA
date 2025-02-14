# 📌 Casos de Teste - Desafio QA

## 🏦 **Testes Funcionais**
### ✅ **Depósito**
#### **CT001 - Depósito Válido**
- **Pré-condição**: O usuário deve estar logado.
- **Passos**:
  1. Acessar a página de depósito.
  2. Inserir um valor válido (ex: R$ 100,00).
  3. Clicar no botão "Depositar".
- **Resultado Esperado**: O saldo deve ser atualizado corretamente e um aviso de sucesso deve ser exibido.

#### ❌ **CT002 - Depósito com Valor Negativo**
- **Pré-condição**: O usuário deve estar logado.
- **Passos**:
  1. Acessar a página de depósito.
  2. Inserir um valor negativo (ex: R$ -100,00).
  3. Clicar no botão "Depositar".
- **Resultado Esperado**: O sistema deve exibir uma mensagem de erro e impedir o depósito.

---

### ✅ **Saque**
#### **CT003 - Saque Válido**
- **Pré-condição**: O usuário deve ter saldo suficiente.
- **Passos**:
  1. Acessar a página de saque.
  2. Inserir um valor dentro do saldo disponível (ex: R$ 50,00).
  3. Clicar no botão "Sacar".
- **Resultado Esperado**: O saldo deve ser atualizado corretamente e uma mensagem de sucesso deve ser exibida.

#### ❌ **CT004 - Saque acima do Saldo**
- **Pré-condição**: O usuário deve ter um saldo menor que o valor a ser sacado.
- **Passos**:
  1. Acessar a página de saque.
  2. Inserir um valor maior que o saldo disponível (ex: R$ 1000,00).
  3. Clicar no botão "Sacar".
- **Resultado Esperado**: O sistema deve exibir uma mensagem de erro e impedir a transação.

---

### ✅ **Transferência**
#### **CT005 - Transferência para outra Conta**
- **Pré-condição**: O usuário deve ter saldo suficiente e conhecer o número da conta de destino.
- **Passos**:
  1. Acessar a página de transferência.
  2. Inserir o número da conta de destino.
  3. Inserir um valor válido (ex: R$ 200,00).
  4. Clicar no botão "Transferir".
- **Resultado Esperado**: O saldo do remetente deve ser reduzido e o saldo do destinatário deve ser aumentado corretamente.

#### ❌ **CT006 - Transferência para Conta Inexistente**
- **Pré-condição**: O usuário deve estar logado.
- **Passos**:
  1. Acessar a página de transferência.
  2. Inserir um número de conta inexistente.
  3. Inserir um valor válido.
  4. Clicar no botão "Transferir".
- **Resultado Esperado**: O sistema deve exibir um erro informando que a conta não existe.

---

## 🎨 **Testes de Interface (UI)**
#### **CT007 - Responsividade no Mobile**
- **Passos**:
  1. Acessar o site em um dispositivo móvel ou reduzir a tela do navegador.
  2. Navegar pelas funcionalidades do site.
- **Resultado Esperado**: Todos os elementos devem estar visíveis e utilizáveis corretamente.
