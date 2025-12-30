# BUG-001 – Mensagem genérica em falha de autenticação

**Resumo:**  
A aplicação exibe uma mensagem genérica de erro ao tentar realizar login com credenciais inválidas, sem diferenciar o motivo da falha.

---

## Ambiente
- Sistema: The Internet – Herokuapp
- URL: https://the-internet.herokuapp.com/login
- Navegador: Google Chrome
- Sistema operacional: macOS

---

## Pré-condições
- Acesso à página de login
- Usuário não autenticado

---

## Passos para reprodução
1. Acessar a página de login
2. Informar usuário inválido ou senha inválida
3. Clicar no botão "Login"

---

## Resultado esperado
O sistema deveria informar de forma clara o motivo da falha (usuário inexistente ou senha incorreta), ou apresentar mensagens específicas para cada cenário.

---

## Resultado obtido
O sistema exibe a mesma mensagem genérica de erro para todos os cenários de falha de autenticação.

---

## Severidade
Baixa

## Prioridade
Baixa

---

## Observações
Este comportamento pode impactar a experiência do usuário, mas não impede o funcionamento da aplicação.
