# Atividade 2 — Organização da Qualidade no LocalEats

**Integrante(s):** [Murilo Rodrigues]

## Tarefa 1 — Diagnóstico da situação

| Problema identificado | Possível consequência para o produto ou equipe |
|---|---|
| Não existem critérios claros para considerar uma funcionalidade pronta. | Funcionalidades podem ser disponibilizadas sem validação suficiente. |
| Defeitos são identificados, mas nem sempre registrados ou acompanhados. | Problemas podem se repetir ou permanecer sem correção. |
| Não está claro quem pode aprovar a disponibilização de uma nova versão. | Podem ocorrer conflitos ou liberações sem aprovação adequada. |

### A qualidade deve ser responsabilidade exclusiva do QA?

Não. A qualidade deve ser responsabilidade compartilhada por toda a equipe. O QA contribui com planejamento e execução dos testes, os desenvolvedores produzem e revisam código, os analistas esclarecem requisitos e o responsável pelo produto prioriza as necessidades dos usuários. Assim, os defeitos podem ser prevenidos e identificados ao longo do desenvolvimento.

## Tarefa 2 — Papéis e competências

| Papel | Responsabilidades relacionadas à qualidade | Competências técnicas | Competências comportamentais |
|---|---|---|---|
| Responsável pelo produto | Definir prioridades e critérios de aceitação. | Gestão de requisitos e regras de negócio. | Comunicação, organização e tomada de decisão. |
| Analista de sistemas/negócio | Detalhar requisitos e identificar regras e situações alternativas. | Modelagem de requisitos e processos. | Pensamento analítico e atenção aos detalhes. |
| Desenvolvedor | Implementar funcionalidades, corrigir defeitos e criar testes unitários. | Programação, depuração e testes unitários. | Colaboração e responsabilidade. |
| QA/analista de qualidade | Planejar testes, analisar riscos, registrar defeitos e verificar correções. | Técnicas de teste, casos de teste e gestão de defeitos. | Pensamento crítico e comunicação. |
| DevOps | Apoiar automação da entrega e monitoramento das versões. | Integração contínua, implantação e monitoramento. | Organização e colaboração. |

## Tarefa 3 — Matriz RACI

R = Responsável pela execução; A = Aprovador; C = Consultado; I = Informado.

| Atividade de qualidade | Produto | Analista | Desenvolvedor | QA | DevOps |
|---|---|---|---|---|---|
| Definir critérios de aceitação | A | R | C | C | I |
| Revisar requisitos | A | R | C | C | I |
| Implementar funcionalidade | I | C | A/R | C | I |
| Revisar código | I | C | A/R | C | I |
| Criar testes unitários | I | C | A/R | C | I |
| Planejar e executar testes do sistema | I | C | C | A/R | C |
| Registrar e acompanhar defeitos | I | C | C | A/R | I |
| Priorizar correção de defeitos | A | C | C | R | I |
| Aprovar disponibilização da versão | A | I | C | C | R |

Revise a matriz com a equipe: cada atividade precisa ter pelo menos um R e exatamente um A. Ajuste a distribuição se os papéis reais do projeto forem diferentes.

## Lacuna ou conflito encontrado

A falta de definição sobre quem aprova a disponibilização de uma nova versão pode provocar conflitos e permitir uma liberação sem que os critérios de qualidade tenham sido verificados. Para resolver isso, deve ser definido um único aprovador e critérios objetivos de liberação.

## Práticas recomendadas

| Prática | Problema que ajuda a resolver | Papéis envolvidos |
|---|---|---|
| Definir uma *Definition of Done*, incluindo revisão de código e testes necessários. | Critérios pouco claros e funcionalidades com defeitos. | Produto, analista, desenvolvedor e QA. |
| Manter registro compartilhado de defeitos com responsável, prioridade, estado e acompanhamento. | Defeitos sem registro ou acompanhamento. | QA, desenvolvedor, produto e analista. |

## Uso de inteligência artificial

**Ferramenta utilizada:** ChatGPT.  
**Como foi utilizada:** apoio para organizar ideias e elaborar sugestões iniciais para as respostas.  
**Como as respostas foram verificadas:** [descrever como eu conferi e ajustei as sugestões conforme o enunciado e o projeto].
