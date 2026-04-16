<img alt="Infografico" src="infografico.png" style="margin: 15px 0" />

# Documentação Técnica e de Produto na Era da Inteligência Artificial

## Sumário Executivo
A documentação de software evoluiu de um pré-requisito burocrático para um **ativo estratégico central**, comparável aos testes automatizados. Na era da IA, ela fornece o contexto necessário para que modelos de linguagem sejam assertivos na geração e manutenção de código. Este documento detalha a categorização de documentos, o papel vital do **PRD** e como o *Prompt Engineering* transforma a criação de registros técnicos em um processo dinâmico e automatizado.

---

## 1. A Nova Era da Documentação

### 1.1. Ativo de Desenvolvimento
Assim como os testes evitam regressões lógicas, a documentação evita a "regressão de contexto". Ela é a base para que a IA gere código alinhado ao negócio ao longo dos anos.

### 1.2. Transmissão de Contexto
Cada interação com uma IA é como integrar um novo membro ao time. A documentação é o meio mais eficiente de realizar o *onboarding* de agentes de IA no conhecimento do projeto.

### 1.3. Documento Vivo
Com Workflows de IA, a documentação evolui com o código. Alterações em funcionalidades podem disparar atualizações automáticas nos documentos, garantindo que o plano e a construção estejam sempre em sincronia.

---

## 2. Categorização de Documentos e Design Docs

| Tipo | Foco Principal | Descrição |
| :--- | :--- | :--- |
| **Produto** | O quê e Por quê | Define o propósito e o valor gerado (PRD). |
| **Design/Arquitetura** | Como | Define a construção técnica e estrutural. |
| **Infraestrutura** | Onde / Com o quê | Define plataformas, provisionamento e ferramentas. |
| **Operacional** | Manutenção | Orienta como manter a aplicação viva. |
| **Conhecimento** | Metodologia | Diretrizes de trabalho no contexto específico. |

> **Nota:** Design, Arquitetura, Infra, Operação e Conhecimento são coletivamente chamados de **Design Docs**.

---

## 3. Product Requirement Document (PRD)
O PRD fornece o contexto de negócio que a IA não possui intrinsecamente.

### 3.1. Níveis de Granularidade
* **Alto Nível (Macro):** Foca na estratégia: Por que o produto existe? Para quem é?
* **Baixo Nível (Feature):** Recomendado para funcionalidades de alto valor ou complexidade (ex: um sistema de login multi-tenant com compliance).



---

## 4. Estrutura e Seções de um PRD

1.  **Visão e Propósito:** A ideia central.
2.  **Contexto e Oportunidade:** O valor para o usuário/empresa.
3.  **Objetivos e Métricas (KPIs):** Como medir o sucesso (ex: latência P95 < 150ms).
4.  **Escopo:** O que está dentro e o que está fora.
5.  **Requisitos Funcionais e Não Funcionais:** O que o sistema faz vs. como ele performa (Segurança, Disponibilidade).
6.  **Arquitetura e Decisões:** Stack tecnológica (ex: Go, PostgreSQL, Redis) e *trade-offs*.
7.  **Critérios de Aceitação:** Checklist para validação final.

---

## 5. IA e Prompt Engineering na Produção de Documentos

### 5.1. O Prompt de Entrevista
Técnica onde a IA atua como uma entrevistadora, extraindo requisitos através de perguntas estruturadas, sugerindo padrões e validando informações antes da geração final.

### 5.2. Saída Multi-formato
* **Markdown:** Para leitura humana e versionamento em Git.
* **JSON:** Para comunicação estruturada entre agentes de IA, permitindo processamento programático de requisitos.



---

## 6. Conclusão
A documentação estruturada é o combustível da IA. Quanto mais rico o contexto (PRDs e Design Docs), menor a probabilidade de código desalinhado. Transformar informações dispersas em ativos organizados é o diferencial dos engenheiros de elite na era da automação.

### [Assista ao resumo em vídeo](https://github.com/user-attachments/assets/e19766cd-8ffb-415e-bee3-180e21c592ac)
