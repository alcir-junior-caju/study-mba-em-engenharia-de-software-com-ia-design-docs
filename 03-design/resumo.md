<img alt="Infografico" src="infografico.png" style="margin: 15px 0" />

# Documentação de Design e Arquitetura de Software

## Sumário
A documentação atua como um **ativo estratégico** que alinha o time, justifica decisões e fornece o contexto necessário para a utilização eficaz de IA. Este documento detalha a hierarquia que vai do produto (**PRD**) à implementação (**FDD/LLD**), destacando o uso de **ADRs** para registro de decisões e a metodologia de **Deep Research** para garantir densidade técnica e inovação no fluxo de trabalho.

---

## 1. Tipologia e Hierarquia de Documentos Técnicos

A documentação deve ser proporcional à complexidade do problema. Abaixo, a cadeia lógica de detalhamento:

| Sigla | Nome | Foco | Descrição |
| :--- | :--- | :--- | :--- |
| **PRD** | Product Requirement Doc | Negócio | O "quê" e o "porquê" sob a visão do usuário. |
| **HLD** | High Level Design | Arquitetura | Visão panorâmica, componentes e stack técnica. |
| **FDD** | Feature Design Doc | Funcionalidade | Detalhamento técnico e contratos de uma feature. |
| **LLD** | Low Level Design | Implementação | Design patterns, campos de API e lógica interna. |
| **ADR** | Arch. Decision Record | Histórico | Justificativa imutável de uma escolha tecnológica. |
| **RFC** | Request for Comments | Colaboração | Documento para discussão e debate de propostas. |



---

## 2. High Level Design (HLD): O Panorama Geral
Define o terreno onde as funcionalidades serão construídas. Permite que arquitetos compreendam o escopo sem entrar em detalhes de codificação.

**Principais Seções:**
* **Arquitetura Geral:** Descrição de serviços e APIs (preferencialmente usando **Modelo C4**).
* **Fluxo de Requisições:** Como os dados transitam entre módulos.
* **Infraestrutura:** Definição da stack (ex: Go, Redis, Kubernetes).
* **Considerações Transversais:** Estratégias macro de segurança, escalabilidade e observabilidade.

---

## 3. Feature Design Doc (FDD): O Guia do Desenvolvedor
Ocupa a posição intermediária crucial: descreve como implementar uma feature dentro do contexto do HLD.

**Elementos Críticos:**
* **Detalhes de Implementação:** Algoritmos (ex: *Token Bucket* para Rate Limiting).
* **Contratos e Interfaces:** Definição de métodos, headers e payloads.
* **Resiliência:** Estratégias de erro e *fallbacks* (ex: *circuit breaker*).
* **SLIs e Alertas:** Métricas específicas que definem a saúde da funcionalidade.



---

## 4. O Papel da IA no Processo de Documentação
A IA elimina a barreira do "ponto zero", acelerando a criação de rascunhos densos.

* **Prompts de Entrevista:** A IA extrai o conhecimento tácito do engenheiro através de perguntas estruturadas.
* **Contextualização:** A IA performa melhor quando recebe o PRD como entrada para gerar o esqueleto do HLD/FDD.

---

## 5. Metodologia de Deep Research
Para temas complexos, utiliza-se uma fase de pesquisa profunda antes da escrita:

1.  **Fase de Coleta:** Agentes de IA pesquisam bibliotecas, padrões e exemplos reais (ex: melhores práticas de mensageria com RabbitMQ).
2.  **Fase de Adaptação:** O conhecimento bruto é processado para os templates da empresa.
3.  **Resultado:** Identifica-se "o que não sabíamos que não sabíamos", garantindo uma documentação de última geração.

---

## 6. Conclusões e Insights Finais
* **Documentação como Asset:** Permite que a IA gere snippets de código precisos, pois ela "entende" o contrato definido.
* **Cultura de Engenharia:** O uso de **ADRs** diferencia times maduros. Registrar por que escolhemos o banco X em vez do Y evita discussões cíclicas no futuro.
* **Redução de Fricção:** O esforço inicial na documentação reduz drasticamente a dívida técnica e acelera o *onboarding* de novos desenvolvedores.

### [Assista ao resumo em vídeo](https://github.com/user-attachments/assets/faf55236-7fed-48a4-9873-b6c836e0b9b0)
