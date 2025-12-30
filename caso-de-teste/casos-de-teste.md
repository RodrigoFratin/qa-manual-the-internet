## CT-001 – Login com credenciais válidas

**Objetivo:**  
Verificar se o usuário consegue acessar a área segura ao informar usuário e senha válidos.

**Pré-condições:**  
- Usuário com credenciais válidas
- Navegador aberto
- Acesso à internet

**Passos:**
1. Acessar a página de login
2. Informar usuário válido
3. Informar senha válida
4. Clicar no botão "Login"

**Resultado esperado:**  
O sistema deve autenticar o usuário e redirecioná-lo para a página "Secure Area", exibindo a mensagem de sucesso.

**Dados de teste:**
- Usuário: `tomsmith`
- Senha: `SuperSecretPassword!`

**Resultado obtido:**  
O sistema autenticou o usuário e permitiu o acesso à área segura.

**Status:**  
✅ Passou

## Observações

- Durante o login com credenciais válidas, o navegador Chrome exibiu um alerta de segurança relacionado a vazamento de senha.
- O alerta é gerado pelo gerenciador de senhas do navegador e não faz parte do sistema testado.
- O comportamento não impacta a funcionalidade de autenticação.


## CT-002 – Login com senha inválida

**Objetivo:**  
Verificar se o sistema impede o acesso quando o usuário informa uma senha inválida.

**Pré-condições:**  
- Usuário com login válido
- Navegador aberto
- Acesso à internet

**Passos:**
1. Acessar a página de login
2. Informar usuário válido
3. Informar senha inválida
4. Clicar no botão "Login"

**Resultado esperado:**  
O sistema não deve permitir o acesso e deve exibir uma mensagem de erro informando que a senha é inválida.

**Dados de teste:**
- Usuário: `tomsmith`
- Senha: `senhaIncorreta123`


**Resultado obtido:**  
O sistema exibiu mensagem de erro informando que a senha é inválida e não permitiu o acesso à área segura.

**Status:**  
✅ Passou

## CT-003 – Login com usuário inválido

**Objetivo:**  
Verificar se o sistema impede o acesso quando um usuário inválido é informado.

**Pré-condições:**  
- Navegador aberto
- Acesso à internet

**Passos:**
1. Acessar a página de login
2. Informar usuário inválido
3. Informar senha válida
4. Clicar no botão "Login"

**Resultado esperado:**  
O sistema não deve permitir o acesso e deve exibir uma mensagem de erro informando que o usuário é inválido.

**Dados de teste:**
- Usuário: `usuarioInvalido`
- Senha: `SuperSecretPassword!`

**Resultado obtido:**  
O sistema exibiu mensagem de erro informando que o usuário é inválido e não permitiu o acesso à área segura.

**Status:**  
✅ Passou

## CT-004 – Login com campos obrigatórios vazios

**Objetivo:**  
Verificar se o sistema valida o preenchimento dos campos obrigatórios ao tentar realizar o login.

**Pré-condições:**  
- Navegador aberto
- Acesso à internet

**Passos:**
1. Acessar a página de login
2. Deixar os campos "Username" e "Password" em branco
3. Clicar no botão "Login"

**Resultado esperado:**  
O sistema não deve permitir o acesso e deve exibir uma mensagem informando que os campos são obrigatórios ou que o login é inválido.

**Dados de teste:**
- Usuário: (em branco)
- Senha: (em branco)

**Resultado obtido:**  
O sistema não permitiu o acesso e exibiu uma mensagem de erro informando que o login é inválido ao tentar autenticar com os campos em branco.

**Status:**  
✅ Passou

## Observações

- Mesmo sem mensagem específica para “campo obrigatório”, o comportamento está consistente com a regra de segurança do sistema.

## CT-005 – Logout com sucesso

**Objetivo:**  
Verificar se o usuário consegue encerrar a sessão com sucesso após realizar o login.

**Pré-condições:**  
- Usuário autenticado no sistema
- Acesso à página "Secure Area"

**Passos:**
1. Estar logado na aplicação
2. Clicar no botão "Logout"

**Resultado esperado:**  
O sistema deve encerrar a sessão do usuário, redirecioná-lo para a página de login e exibir uma mensagem informando que o logout foi realizado com sucesso.

**Dados de teste:**
- Usuário: `tomsmith`
- Senha: `SuperSecretPassword!`

**Resultado obtido:**  
O sistema encerrou a sessão do usuário com sucesso, redirecionando para a página de login e exibindo a mensagem de logout realizado com sucesso.

**Status:**  
✅ Passou




