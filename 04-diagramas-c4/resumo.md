<img alt="Infografico" src="infografico.png" style="margin: 15px 0" />

# Modelagem de Sistemas e Automação de Diagramas C4 com IA

## Sumário
Este documento sintetiza as diretrizes para a representação visual de arquiteturas de software utilizando o **Modelo C4** e automação via **IA**. A documentação visual é um complemento estratégico aos *Design Docs*, facilitando o alinhamento entre times técnicos e stakeholders. Através da tradução de especificações escritas em código de diagramação (PlantUML/Mermaid), a IA transforma a criação de diagramas de uma tarefa onerosa em um processo ágil e evolutivo.

---

## 1. A Importância da Representação Visual
Diagramas atuam como ferramentas de clareza que quebram a densidade de textos técnicos longos.
* **Alinhamento Multidisciplinar:** Facilita a comunicação com Produto, Segurança e Liderança.
* **Diagrams as Code:** O uso de ferramentas como **Mermaid** (renderização nativa no GitHub) e **PlantUML** permite que diagramas sejam versionados no Git junto com o código.

---

## 2. O Modelo C4: Estrutura e Níveis
Organiza a arquitetura em quatro níveis de abstração, permitindo diferentes profundidades de análise:

| Nível | Nome | Foco Principal | Descrição |
| :--- | :--- | :--- | :--- |
| **C1** | System Context | Visão Externa | Atores, usuários e sistemas externos integrados. |
| **C2** | Containers | Blocos Principais | APIs, Bancos de Dados, Filas e Microserviços. |
| **C3** | Components | Estrutura Interna | Módulos, camadas e responsabilidades dentro de um container. |
| **C4** | Code | Detalhe Técnico | Classes, interfaces e structs (geralmente gerado via IA). |

### Estudo de Caso: Rate Limiter
* **C1:** Define o SDK interagindo com desenvolvedores e sistemas de monitoramento.
* **C2:** Mostra o serviço em Go, o armazenamento distribuído no **Redis** e o scraping pelo **Prometheus**.
* **C3:** Detalha o *Middleware HTTP*, o *Strategy Engine* (algoritmos) e o *Storage Adapter*.

---

## 3. Automação com Inteligência Artificial
A IA não inventa a arquitetura; ela **traduz** o seu *Feature Design Document (FDD)* para uma linguagem visual.

* **FDD como Fonte da Verdade:** A qualidade do diagrama é diretamente proporcional à precisão do documento escrito.
* **Linguagens de Marcação:** A IA gera arquivos `.puml` (PlantUML) ou `.mmd` (Mermaid), que podem ser convertidos instantaneamente em imagens.
* **Workflow Ágil:** Ferramentas como **Cursor** ou **Claude Code** utilizam prompts estruturados para identificar até qual nível de detalhe (C1-C4) a informação disponível permite chegar.

---

## 4. Estrutura de Prompts Eficazes
Para gerar diagramas precisos, o prompt deve exigir:
1.  **Fidelidade ao Contexto:** Usar apenas os componentes definidos no documento de referência.
2.  **Padrão C4:** Instruções explícitas para usar bibliotecas C4-PlantUML (`C4_Context.puml`, `C4_Container.puml`).
3.  **Encoding e Idioma:** Garantir suporte a UTF-8 para acentuação e manter termos técnicos em inglês conforme o padrão da indústria.

---

## 5. Considerações Práticas e Fluxo de Trabalho
* **IA como Rascunho:** O diagrama gerado é uma base que deve passar por revisão humana.
* **Sincronização:** Com a automação, é possível atualizar os diagramas em segundos sempre que o FDD ou a arquitetura mudar.
* **Julgamento Profissional:** O nível **C4 - Code** deve ser usado com parcimônia, apenas quando a lógica interna for crítica para a compreensão de segurança ou auditoria.

---
> "O diagrama C4 é o mapa; o Design Doc é o guia de viagem. A IA é o motor que permite manter ambos atualizados em tempo real."

### [Assista ao resumo em vídeo](https://github.com/user-attachments/assets/b68f02bb-3689-4afb-8955-a576f15372a3)
