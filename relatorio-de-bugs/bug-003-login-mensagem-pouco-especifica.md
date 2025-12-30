# BUG-003 – Mensagem de erro pouco específica no login

## Resumo
Mensagem de erro exibida no login não diferencia usuário inexistente
de senha incorreta.

## Ambiente
- Site: The Internet (Herokuapp)
- Navegador: Chrome
- Sistema Operacional: macOS Big Sur 11.7.10

## Passos para Reproduzir
1. Acessar a página de login
2. Inserir usuário inválido
3. Inserir senha inválida
4. Clicar em "Login"

## Resultado Atual
Mensagem genérica: "Your username is invalid!"

## Resultado Esperado
Mensagem mais específica ou orientação clara ao usuário,
indicando qual campo está incorreto.

## Severidade
Baixa

## Prioridade
Baixa

## Observações
Bug levantado a partir de teste exploratório.
