# Relatório Final de Testes

## 1. Introdução
Este documento apresenta os resultados dos testes manuais realizados no sistema 
"The Internet", disponível em https://the-internet.herokuapp.com/.

O objetivo foi validar funcionalidades principais relacionadas ao login, 
mensagens de erro e comportamento do sistema frente a entradas inválidas.

---

## 2. Escopo dos Testes
Foram testadas as seguintes funcionalidades:
- Autenticação de usuário (login)
- Validação de credenciais inválidas
- Mensagens de erro exibidas ao usuário
- Comportamento do sistema após tentativas incorretas

Funcionalidades fora do escopo:
- Testes de performance
- Testes de segurança
- Testes automatizados

---

## 3. Ambiente de Testes
- Sistema Operacional: macOS Big Sur 11.7.10
- Navegador: Google Chrome (última versão compatível)
- Tipo de teste: Testes manuais funcionais e exploratórios
- Ambiente: Produção (site público)

---

## 4. Estratégia de Testes
A estratégia adotada incluiu:
- Casos de teste baseados em requisitos implícitos
- Testes exploratórios focados em experiência do usuário
- Execução manual com validação visual das respostas do sistema

---

## 5. Casos de Teste Executados
Total de casos de teste executados: **05**

| ID do Caso | Descrição | Resultado |
|-----------|----------|----------|
| CT-001 | Login com credenciais válidas | Passou |
| CT-002 | Login com senha inválida | Passou |
| CT-003 | Login com usuário inválido | Passou |
| CT-004 | Campos em branco no login | Passou |
| CT-005 | Teste exploratório de mensagens | Passou |

---

## 6. Bugs Encontrados

| ID do Bug | Título | Severidade | Status |
|----------|------|------------|--------|
| BUG-001 | Mensagem genérica para login inválido | Média | Aberto |
| BUG-002 | Feedback pouco claro ao usuário | Baixa | Aberto |
| BUG-003 | Mensagem de erro pouco específica no login | Baixa | Aberto |

---

## 7. Avaliação da Qualidade
O sistema apresentou comportamento estável e consistente durante os testes.
As funcionalidades principais funcionam conforme o esperado.

Os problemas encontrados estão relacionados principalmente à **experiência do usuário**, 
especialmente na clareza das mensagens de erro.

---

## 8. Conclusão
Com base nos testes realizados, o sistema está **funcional para uso básico**, 
porém recomenda-se melhorias nas mensagens exibidas ao usuário para aumentar 
a usabilidade e reduzir possíveis confusões durante o processo de login.
