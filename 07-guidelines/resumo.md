<img alt="Infografico" src="infografico.png" style="margin: 15px 0" />

# Diretrizes de Desenvolvimento de Software: Guia de Implementação e Uso de IA

## Sumário Executivo
As **Software Development Guidelines** configuram-se como um pilar estratégico para a governança técnica. Na engenharia moderna, elas servem como um "mapa do saber" para alinhar desenvolvedores e agentes de IA, mitigando ruídos em revisões de código e garantindo que a evolução do sistema seja consistente e previsível.

---

## 1. Definição e Escopo das Guidelines
Diferente de um simples guia de estilo, as diretrizes orientam a escrita, organização e evolução do código em um contexto específico.
* **Abrangência:** Cobre linguagens, frameworks, padrões de arquitetura e segurança.
* **Propósito:** Definir o "como" desenvolvemos, garantindo que o software seja manutenível independentemente de quem (ou o quê) o escreva.

---

## 2. O Papel Estratégico da IA no Desenvolvimento
A integração da IA transforma as *guidelines* em ferramentas de **onboarding automático**.

### Benefícios da IA Orientada por Guidelines
* **Injeção de Conhecimento:** Permite que a IA entenda os processos internos do time imediatamente.
* **Redução de Ruídos em Code Review:** Evita refatorações desnecessárias sugeridas pela IA que fogem do padrão do projeto.
* **Minimização de Erros:** Facilita a criação de *hooks* de pré-commit automatizados, mitigando alucinações técnicas.

---

## 3. Estrutura Fundamental de um Documento de Guidelines

| Seção | Descrição |
| :--- | :--- |
| **Core Principles** | Princípios inegociáveis (ex: SOLID, Simplicidade). |
| **Project Stack** | Definição de linguagens, frameworks, ORMs e libs de teste. |
| **Convenções de Código** | Nomenclatura, tipagem, tratamento de erros e comentários. |
| **Estrutura de Projeto** | Organização de diretórios e padrões arquiteturais. |
| **Testes e Qualidade** | Padrões para unitários, integração, mocks e linting. |
| **Observabilidade** | Estruturação de logs (Pino/Winston), métricas e tracing. |

### Golden Rules e Checklists
As "Regras de Ouro" alimentam a **Checklist Pré-commit**. Antes de cada entrega, a IA ou o dev verificam:
1. O código compila sem warnings?
2. Os testes passaram com a cobertura mínima?
3. A documentação (README/Swagger) foi atualizada?

---

## 4. Metodologia de Geração de Guidelines via IA
A geração desses documentos deve ser incremental para garantir densidade e evitar perda de contexto:

1.  **Fase de Parsing:** Identificação automática da stack atual.
2.  **Fase de Pesquisa:** Consolidação de padrões de mercado (ex: Google Style Guide).
3.  **Geração Incremental:** Escrita por blocos para não estourar a janela de contexto.
4.  **Autovalidação:** Revisão pelo agente para remover verbosidade e garantir aplicabilidade.

---

## 5. Categorização de Design Docs
As *guidelines* inserem-se no ecossistema de documentação técnica como documentos de **Conhecimento e Referência**, servindo de base para:
* **Design e Arquitetura:** Onde as diretrizes são aplicadas na prática.
* **Operações:** Onde os padrões de log e observabilidade definidos nas *guidelines* são consumidos.

---

> "Instruções extremamente claras e uma estrutura onde o agente de IA consiga se autoavaliar são essenciais. Se isso não estiver claro, simplesmente não funciona."

### [Assista ao resumo em vídeo](https://github.com/user-attachments/assets/8226d42c-0956-41b8-a55e-b15ee151233f)
