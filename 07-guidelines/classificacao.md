# Mindmap: Classificação Geral de Documentos Técnicos (Era Moderna)

## 1. Documentos de Relevância Crítica (The "Gold Standard")

Esta categoria contém os documentos indispensáveis para o sucesso de qualquer projeto de software resiliente e orientado a IA.

| Documento | Categoria | Características e Valor Estratégico |
| :--- | :--- | :--- |
| **PRD** (Product Requirements Document) | **Produto** | O "Quê" e o "Porquê". Liga a visão de negócio à execução. É leve e focado em métricas. |
| **HLD** (High-Level Design) | **Arquitetura** | O "Como" macro. Define o alicerce técnico e as integrações principais. |
| **FDD** (Feature Design Doc) | **Arquitetura** | O "Como" micro. Sucessor do FRD, focado em clareza de implementação para o desenvolvedor. |
| **ADR** (Architecture Decision Record) | **Arquitetura** | Padrão ouro de governança. Registra o histórico e os trade-offs de decisões passadas. |
| **RFC** (Request for Comments) | **Arquitetura** | Documento colaborativo para discussões assíncronas e consenso técnico. |
| **Modelos C4** | **Arquitetura** | Padrão visual moderno (Context, Container, Component, Code). Simples e versionável. |
| **Runbooks / Playbooks** | **Operacional** | O manual de sobrevivência em incidentes (DevOps/SRE). |
| **Engineering Guidelines** | **Referência** | Centralizam a cultura técnica (Style guides, CI/CD, Segurança). |
| **Security Design Doc** | **Referência** | Focado em Threat Modeling, Autenticação e Compliance. |



---

## 2. Documentos Emergentes e Modernos (Era da IA & SRE)

Novas fronteiras que surgiram com a necessidade de medir e operar sistemas inteligentes e distribuídos.

| Documento | Categoria | Observação |
| :--- | :--- | :--- |
| **AI Design / Prompt Specs** | **Arquitetura** | Documentação de fluxos de agentes, cadeias de pensamento (CoT) e versões de prompts. |
| **Evaluation Docs** | **Referência** | Medição de precisão (F1-Score, Precisão, Recall), custo e alucinações em LLMs. |
| **Observability Docs** | **Operacional** | Define SLIs, SLOs e como as métricas se ligam ao valor de negócio. |

---

## 3. Documentos Secundários (Apoio)

Documentos que ainda possuem valor, mas que muitas vezes têm sua função absorvida pelo código ou por outras ferramentas.

*   **LLD (Low-Level Design):** Relevante apenas em núcleos críticos (algoritmos complexos). Caso contrário, código e ADRs bastam.
*   **Infrastructure Design Doc:** Parte substancial hoje vive como **IaC** (Terraform/CloudFormation).
*   **User Stories & Epics:** Essenciais para gestão ágil (Jira/Linear), mas não substituem o detalhamento técnico do PRD/FDD.
*   **CI/CD Documentation:** Geralmente vive dentro dos arquivos de workflow (YAML) no repositório.

---

## 4. Legado e Herança Waterfall (Baixa Relevância)

Documentos que perderam espaço devido à sua rigidez e alto custo de manutenção, sendo substituídos por versões mais enxutas.

| Documento | Categoria | Motivo da Obsolescência |
| :--- | :--- | :--- |
| **FRD** (Functional Req. Doc) | **Produto** | Muito pesado. Substituído pela dupla PRD + FDD. |
| **TRD** (Technical Ref. Doc) | **Arquitetura** | Substituído por specs automáticas (OpenAPI/Swagger, Protobuf). |
| **UML Extenso (RUP)** | **Arquitetura** | Diagramas excessivamente detalhados deram lugar ao pragmatismo do Modelo C4. |
| **Test Plan Formal** | **Referência** | Substituído por testes automatizados, TDD e pipelines de CI. |



---

## Conclusão: O "Kit Sobrevivência" do Desenvolvedor Moderno

Para um projeto saudável hoje, o foco deve estar na **Trindade da Documentação Ativa**:
1.  **PRD** para entender o negócio.
2.  **FDD/HLD** com **C4** para entender a construção.
3.  **ADRs** para entender a evolução e os motivos das escolhas.
