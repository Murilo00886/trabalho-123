# Atividade 1 — Fundamentos e Características da Qualidade no LocalEats

**Integrante(s):** [Murilo Rodrigues]  
**Projeto:** LocalEats

## Tarefa 1 — Fundamentos da qualidade

| Tipo | Necessidade | Interessado | Consequência se não for atendida |
|---|---|---|---|
| Explícita | Criar uma conta e entrar no sistema. | Usuário | O usuário pode não conseguir acessar as funcionalidades que exigem autenticação. |
| Explícita | Pesquisar restaurantes por especialidade ou localização. | Usuário | O usuário terá dificuldade para encontrar restaurantes adequados ao que procura. |
| Implícita | Proteger os dados e as credenciais dos usuários. | Usuário e empresa | Pode ocorrer exposição de informações e perda de confiança. |
| Implícita | Apresentar resultados e informações de pedidos corretos. | Usuário e restaurante | O usuário pode tomar decisões com base em informações incorretas. |

### Um sistema que implementa todas as funcionalidades explicitamente solicitadas pode ainda apresentar baixa qualidade?

Sim. Um sistema pode implementar todas as funcionalidades solicitadas e ainda apresentar baixa qualidade se não atender às necessidades implícitas dos usuários. Por exemplo, pode permitir a criação de contas, mas não proteger adequadamente as credenciais. Portanto, a qualidade também depende de segurança, confiabilidade e satisfação dos usuários.

## Tarefa 2 — Exploração da aplicação

**Funcionalidade escolhida:** Login.

| Integrante | Funcionalidade | O que foi realizado | O que foi observado | Evidência |
|---|---|---|---|---|
| [Murilo Rodrigues] | Login | Foi apresentada uma captura da tela inicial com sessão identificada como “Olá, John” e outra captura da tela de login com mensagem “Invalid credentials”. Confirmar se essas telas correspondem às tentativas realizadas. | Na tela de login aparece a mensagem “Invalid credentials”. A outra captura mostra a página de exploração com o usuário “John”. Não inferir além do que as imagens comprovam. | `evidencias/testes-login-juntos.png` |

**Atenção:** complete esta tabela com o que você realmente fez e observou. Se realizou um login válido e uma tentativa inválida, descreva cada tentativa com precisão.

## Tarefa 3 — Requisito e característica de qualidade

| Integrante | Requisito de qualidade | Característica/subcaracterística | Justificativa | Como avaliar |
|---|---|---|---|---|
| [Murilo Rodrigues] | O sistema deve impedir o acesso quando as credenciais forem inválidas e apresentar uma mensagem clara ao usuário. | Segurança — autenticidade | O login deve verificar as credenciais antes de permitir acesso à conta. | Tentar entrar com credenciais válidas e inválidas, observar se o acesso é permitido apenas quando a autenticação é bem-sucedida e registrar as mensagens apresentadas. |

## Evidências

As capturas fornecidas foram reunidas em `evidencias/testes-login-juntos.png`.
