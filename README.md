[test-cases.md](https://github.com/user-attachments/files/26951828/test-cases.md)
# test-cases
README + 8 casos de teste completos para login
# Casos de Teste — Login

---

## TC-001 — Login com credenciais válidas

| Campo | Detalhe |
|---|---|
| **ID** | TC-001 |
| **Tipo** | ✅ Positivo |
| **Prioridade** | Alta |

**Pré-condição:** Usuário cadastrado com email e senha válidos.

**Passos:**
1. Acessar a página de login
2. Inserir email válido
3. Inserir senha correta
4. Clicar em "Entrar"

**Resultado Esperado:** Usuário redirecionado para a página inicial autenticado.

**Status:** ⏳ Não executado

---

## TC-002 — Login com senha incorreta

| Campo | Detalhe |
|---|---|
| **ID** | TC-002 |
| **Tipo** | ❌ Negativo |
| **Prioridade** | Alta |

**Pré-condição:** Usuário cadastrado com email válido.

**Passos:**
1. Acessar a página de login
2. Inserir email válido
3. Inserir senha incorreta
4. Clicar em "Entrar"

**Resultado Esperado:** Mensagem de erro exibida. Usuário não autenticado.

**Status:** ⏳ Não executado

---

## TC-003 — Login com email não cadastrado

| Campo | Detalhe |
|---|---|
| **ID** | TC-003 |
| **Tipo** | ❌ Negativo |
| **Prioridade** | Alta |

**Pré-condição:** Nenhuma.

**Passos:**
1. Acessar a página de login
2. Inserir email não cadastrado
3. Inserir qualquer senha
4. Clicar em "Entrar"

**Resultado Esperado:** Mensagem de erro exibida. Usuário não autenticado.

**Status:** ⏳ Não executado

---

## TC-004 — Login com campos vazios

| Campo | Detalhe |
|---|---|
| **ID** | TC-004 |
| **Tipo** | ❌ Negativo |
| **Prioridade** | Média |

**Pré-condição:** Nenhuma.

**Passos:**
1. Acessar a página de login
2. Deixar campos em branco
3. Clicar em "Entrar"

**Resultado Esperado:** Campos obrigatórios destacados. Botão bloqueado ou mensagem de validação exibida.

**Status:** ⏳ Não executado

---

## TC-005 — Login com email em formato inválido

| Campo | Detalhe |
|---|---|
| **ID** | TC-005 |
| **Tipo** | ❌ Negativo |
| **Prioridade** | Média |

**Pré-condição:** Nenhuma.

**Passos:**
1. Acessar a página de login
2. Inserir "usuario@" no campo de email
3. Inserir qualquer senha
4. Clicar em "Entrar"

**Resultado Esperado:** Validação de formato de email ativada. Login não realizado.

**Status:** ⏳ Não executado

---

## TC-006 — Bloqueio após 3 tentativas inválidas

| Campo | Detalhe |
|---|---|
| **ID** | TC-006 |
| **Tipo** | 🔍 Exploratório |
| **Prioridade** | Alta |

**Pré-condição:** Usuário cadastrado.

**Passos:**
1. Tentar login com senha errada 3 vezes consecutivas
2. Observar comportamento do sistema na 4ª tentativa

**Resultado Esperado:** Conta bloqueada temporariamente ou CAPTCHA ativado.

**Status:** ⏳ Não executado

---

## TC-007 — Login com espaços antes/depois das credenciais

| Campo | Detalhe |
|---|---|
| **ID** | TC-007 |
| **Tipo** | 🔍 Exploratório — Edge Case |
| **Prioridade** | Baixa |

**Pré-condição:** Usuário cadastrado.

**Passos:**
1. Inserir " usuario@email.com " (com espaços)
2. Inserir senha correta
3. Clicar em "Entrar"

**Resultado Esperado:** Sistema faz trim dos espaços e autentica normalmente, ou exibe mensagem de validação.

**Status:** ⏳ Não executado

---

## TC-008 — Visibilidade da senha

| Campo | Detalhe |
|---|---|
| **ID** | TC-008 |
| **Tipo** | ✅ Positivo |
| **Prioridade** | Baixa |

**Pré-condição:** Nenhuma.

**Passos:**
1. Acessar a página de login
2. Digitar qualquer texto no campo de senha
3. Clicar no ícone de "olho" para exibir senha

**Resultado Esperado:** Senha exibida em texto plano ao clicar no ícone.

**Status:** ⏳ Não executado
