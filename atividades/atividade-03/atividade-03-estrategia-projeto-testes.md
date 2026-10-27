# Atividade 3 — Estratégia e Projeto de Testes do LocalEats

**Integrante(s):** [Murilo Rodrigues]  
**Funcionalidade de exemplo:** Pesquisa de restaurantes

> Este arquivo é um modelo inicial. Ajuste a funcionalidade e a quantidade de riscos/casos conforme a modalidade individual ou em equipe.

## Tarefa 1 — Planejamento dos testes

### 1.1 Objetivo dos testes

Verificar se o LocalEats permite pesquisar restaurantes por especialidade ou localização, apresenta resultados compatíveis com os critérios informados e trata adequadamente pesquisas sem resultados ou com entradas inválidas.

### 1.2 Escopo

| Incluído | O que será verificado |
|---|---|
| Pesquisa por especialidade | Se os resultados correspondem à especialidade informada. |
| Pesquisa por localização | Se os resultados correspondem à localização pesquisada. |

**Fora do escopo:** realização de pedidos, pois este plano se concentra na pesquisa de restaurantes.

### 1.3 Abordagem

| Item | Definição | Justificativa |
|---|---|---|
| Nível de teste | Sistema | A funcionalidade será avaliada pela interface da aplicação. |
| Tipo de teste | Funcional | Serão verificados regras e resultados da pesquisa. |
| Perspectiva | Caixa-preta | Serão avaliadas entradas e saídas sem analisar o código. |
| Técnica 1 | Particionamento de equivalência | Permite testar classes de entradas representativas. |
| Técnica 2 | Análise de valor limite, se houver limites definidos | Verifica valores próximos aos limites de uma regra. |

### 1.4 Ambiente e responsabilidades

| Item | Definição |
|---|---|
| Ambiente | Aplicação LocalEats, navegador atualizado, dispositivo com internet e dados de restaurantes disponíveis. |
| Planejamento | [] |
| Especificação dos casos | [] |
| Futura execução | [] |

### 1.5 Critérios

| Critério | Definição |
|---|---|
| Entrada | Aplicação acessível e dados de restaurantes disponíveis. |
| Saída | Casos planejados executados futuramente e resultados registrados. |
| Suspensão | Aplicação indisponível ou ausência de dados necessários para avaliar os resultados. |

## Tarefa 2 — Análise dos riscos

| ID | Integrante | Funcionalidade | Risco | Consequência | Probabilidade | Impacto | Prioridade | Justificativa |
|---|---|---|---|---|---|---|---|---|
| R01 | [Murilo] | Pesquisa por especialidade | A pesquisa apresenta restaurantes que não correspondem à especialidade informada. | Usuário pode escolher um restaurante inadequado. | Média | Alto | Alta | A inconsistência prejudica diretamente a utilidade da pesquisa. |
| R02 | [Murilo] | Pesquisa por localização | A pesquisa não encontra restaurantes existentes na localização informada. | Usuário pode acreditar que não existem opções disponíveis. | Média | Médio | Média | Resultados incompletos reduzem a confiança na aplicação. |

As classificações são estimativas de planejamento, não defeitos observados.

## Tarefa 3 — Casos de teste

### CT01 — Pesquisar especialidade existente

- **Integrante responsável:** [Murilo]
- **Funcionalidade:** pesquisa por especialidade
- **Risco relacionado:** R01
- **Técnica:** particionamento de equivalência
- **Pré-condição:** aplicação acessível e existência de restaurantes cadastrados na especialidade escolhida.
- **Dados de entrada:** especialidade existente, como pizza, se estiver cadastrada.
- **Passos:**
  1. Abrir o LocalEats.
  2. Acessar a pesquisa de restaurantes.
  3. Informar a especialidade escolhida.
  4. Executar a pesquisa.
  5. Conferir os resultados.
- **Resultado esperado:** os restaurantes apresentados correspondem à especialidade pesquisada.

### CT02 — Pesquisar especialidade sem resultados

- **Integrante responsável:** [Murilo]
- **Funcionalidade:** pesquisa por especialidade
- **Risco relacionado:** R01
- **Técnica:** particionamento de equivalência
- **Pré-condição:** aplicação acessível e termo sem correspondência nos dados disponíveis.
- **Dados de entrada:** especialidade inexistente no catálogo utilizado para o teste.
- **Passos:**
  1. Abrir a pesquisa de restaurantes.
  2. Informar o termo escolhido.
  3. Executar a pesquisa.
  4. Observar a resposta.
- **Resultado esperado:** a aplicação informa que não há resultados ou apresenta estado vazio adequado, sem exibir restaurantes incompatíveis.

### CT03 — Pesquisar por localização

- **Integrante responsável:** [Murilo]
- **Funcionalidade:** pesquisa por localização
- **Risco relacionado:** R02
- **Técnica:** particionamento de equivalência
- **Pré-condição:** aplicação acessível e existência de restaurantes cadastrados na localização escolhida.
- **Dados de entrada:** localização com restaurantes cadastrados.
- **Passos:**
  1. Abrir a pesquisa de restaurantes.
  2. Informar a localização escolhida.
  3. Executar a pesquisa.
  4. Conferir os restaurantes apresentados.
- **Resultado esperado:** a aplicação apresenta os restaurantes correspondentes à localização informada.

## Matriz de rastreabilidade

| Integrante | Funcionalidade | Risco/requisito | Técnica | Casos de teste |
|---|---|---|---|---|
| [Murilo] | Pesquisa por especialidade | R01 — resultados incompatíveis | Particionamento de equivalência | CT01 e CT02 |
| [Murilo] | Pesquisa por localização | R02 — resultados incompletos | Particionamento de equivalência | CT03 |

## Uso de inteligência artificial

**Ferramenta utilizada:** ChatGPT.  
**Como foi utilizada:** apoio para organizar o plano, riscos e casos de teste.  
**Uma sugestão que precisou ser alterada ou rejeitada:**   
**Como as respostas foram verificadas:** [descrever a conferência com o enunciado e a aplicação].
