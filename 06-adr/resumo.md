<img alt="Infografico" src="infografico.png" style="margin: 15px 0" />

# Architecture Decision Record (ADR): O Guia Definitivo para Documentação e Evolução Arquitetural

## Sumário Executivo
Este documento sintetiza os conceitos, práticas e metodologias para a implementação de **Architecture Decision Records (ADR)**. O ADR é identificado como um registro histórico vivo das motivações por trás das decisões arquiteturais significativas. Ao focar no **"porquê"** em vez de apenas no **"o quê"**, as ADRs garantem a continuidade do conhecimento, facilitam o *onboarding* e fornecem contexto crítico para que ferramentas de IA operem com maior assertividade. A adoção do padrão **MADR (Markdown ADR)** e a automação via agentes de IA representam o estado da arte na gestão de conhecimento técnico.

---

## 1. O Conceito e o Valor da ADR
O ADR é um documento curto e objetivo que captura uma decisão arquitetural importante, incluindo seu contexto e as consequências da escolha feita.

*   **Memória Organizacional:** Preserva a linha de raciocínio original, evitando que decisões pareçam aleatórias após anos de evolução do sistema.
*   **Foco no Trade-off:** Documenta as alternativas descartadas e as justificativas técnicas, estratégicas ou de negócio.
*   **Complementaridade:** Enquanto o PRD define o que será feito e o HLD como será estruturado, o ADR explica a **razão técnica** da escolha.
*   **Aliado da IA:** Permite que IAs compreendam o contexto temporal, sugerindo soluções alinhadas à evolução histórica do projeto.

---

## 2. Estrutura e Padronização

### 2.1. O Modelo Clássico (Michael Nygard)
1.  **Título:** Nome claro da decisão.
2.  **Status:** Estado atual (ex: proposto, aceito).
3.  **Contexto:** O problema ou situação que motivou a decisão.
4.  **Decisão:** A escolha técnica propriamente dita.
5.  **Consequências:** Os resultados (positivos e negativos) da aplicação.

### 2.2. MADR: Markdown ADR
O MADR é otimizado para ser legível por humanos e processável por máquinas, utilizando metadados rigorosos.

| Metadado | Descrição |
| :--- | :--- |
| **Status** | Proposed, Accepted, Rejected, Deprecated ou Superseded. |
| **Supersedes** | Aponta qual ADR antiga está sendo substituída por esta. |
| **Superseded by** | Link para a nova ADR que substitui o documento atual. |
| **Amends** | Indica que a ADR atual corrige ou complementa uma anterior. |

---

## 3. Critérios de Aplicação: Quando Gerar uma ADR
Utilize a **Regra dos 3 Es**: a decisão é **Estrutural**, **Evidente** (importante para outros no futuro) e **Estável** (longa duração)?

### 3.1. Uso Recomendado (Must)
*   **Tecnologias Base:** Linguagens, frameworks, bancos de dados e mensageria.
*   **Padrões de Comunicação:** REST, gRPC, Event-driven.
*   **Estratégias de Persistência:** SQL vs NoSQL, consistência, caching.
*   **Segurança e Infra:** Protocolos Auth, Kubernetes, provedores de Cloud.

### 3.2. Quando Não Usar (Ruído)
*   Logs operacionais ou refatorações de baixo impacto.
*   Configurações triviais (linters, formatação).
*   Bugs e hotfixes (pertencem a *incident reports*).

---

## 4. O Ciclo de Vida e Fluxo de Trabalho
O gerenciamento segue um fluxo dinâmico:
1.  **Draft/Proposed:** Rascunho inicial (geralmente vindo de uma RFC).
2.  **Review:** Debate entre o time e *Tech Leads*.
3.  **Accepted/Rejected:** Registro da aprovação ou recusa (importante para não repetir erros).
4.  **Superseded:** Quando algo novo substitui a decisão, a ADR antiga é marcada como tal e uma nova é criada, preservando a **linha do tempo**.

---

## 5. IA e Automação: O Futuro da Documentação
Agentes de IA podem mapear sistemas legados em quatro fases:
1.  **ADR Analyzer:** Mapeia o codebase e gera um `mapping.md`.
2.  **Identificação:** IA aponta o que "deve ser documentado" vs "pode ser documentado".
3.  **ADR Generator:** Gera o MADR com marcações de *"Needs Input"* para contextos que só humanos possuem (decisões de custo ou negócio).
4.  **ADR Linker:** Estabelece conexões automáticas de dependência e substituição entre documentos.

---

## 6. Melhores Práticas
*   **Uma decisão por ADR:** Evite agrupar escolhas não relacionadas.
*   **Linguagem Natural:** Foco em humanos e IAs; evite jargões excessivos.
*   **Evite Código Direto:** Foque em conceitos arquiteturais, não em detalhes de implementação voláteis.
*   **Qualidade sobre Quantidade:** A IA fornece o ponto de partida, mas a revisão humana é o filtro final.

### [Assista ao resumo em vídeo](https://github.com/user-attachments/assets/6592dd09-7408-41a0-b684-51f81d10f43b)
