<img alt="Infografico" src="infografico.png" style="margin: 15px 0" />

# Mermaid: Linguagem de Marcação e Automação de Diagramas Técnicos

## Sumário
Este documento detalha o uso do Mermaid como uma solução eficiente para a visualização de sistemas, fluxos de decisão e estruturas de dados. O Mermaid se destaca por ser uma linguagem de marcação que converte texto em diagramas, eliminando a necessidade de ferramentas gráficas pesadas e facilitando a manutenção via código. Sua principal vantagem reside na simplicidade e na integração nativa com arquivos Markdown em plataformas como o GitHub. A integração com Inteligência Artificial (IA) permite a geração automatizada e a atualização contínua de diagramas a partir de documentos técnicos, garantindo que a documentação acompanhe a evolução do código com baixo esforço manual.

---

## 1. Visão Geral do Mermaid
O Mermaid é definido como uma linguagem de marcação projetada para transformar texto legível em representações gráficas. Ele é amplamente utilizado para documentar fluxos, integrações e estruturas de sistemas.

### Diferenciais e Vantagens
* **Simplicidade e Baixa Verbosidade**: Comparado ao PlantUML, o Mermaid é menos detalhado e extenso, focando na facilidade de escrita e leitura do código-fonte do diagrama.
* **Integração com Markdown**: Diferente do modelo C4, que muitas vezes exige a gestão de arquivos de imagem externos, o Mermaid é renderizado automaticamente em arquivos Markdown (como README.md) em plataformas como GitHub.
* **Facilidade de Manutenção**: Por ser baseado em texto, facilita a revisão por pares, o controle de versão e a automação por agentes de IA.
* **Flexibilidade**: Pode ser utilizado para representar desde regras de negócio específicas até arquiteturas de alto nível, embora sua força resida na capacidade de detalhar componentes técnicos.

---

## 2. Tipos de Diagramas e Aplicações
O Mermaid suporta diversos tipos de diagramas, cada um adequado a uma necessidade específica de documentação:

### 2.1 Flowchart (Fluxograma)
Representa fluxos de decisão, etapas de processos e caminhos alternativos.
* **Uso Ideal**: Lógica de processos, pipelines e documentação de APIs.
* **Exemplo Prático**: Verificação de chaves em um Rate Limiter, distinguindo o fluxo entre armazenamento em Redis (usando scripts Lua) ou em Memória (usando Mutex e LocalMap).

### 2.2 Sequence Diagram (Diagrama de Sequência)
Visualiza a troca de mensagens entre componentes ao longo do tempo.
* **Uso Ideal**: Chamadas entre serviços, interações com bancos de dados e identificação de gargalos de comunicação.
* **Exemplo Prático**: O fluxo de uma requisição HTTP que passa por um middleware, consulta o Rate Limiter, interage com o storage e retorna status 200 (Sucesso) ou 429 (Too Many Requests).

### 2.3 Class Diagram (Diagrama de Classes)
Oferece um nível mais baixo de abstração, expondo a estrutura interna do código.
* **Uso Ideal**: Explicar o design do domínio, atributos, métodos, heranças e relacionamentos entre structs ou classes.
* **Exemplo Prático**: Representação de uma struct `options` em Go para configurar estratégias de janela e limites de um sistema.

### 2.4 Entity-Relationship Diagram (ER)
Foca nas estruturas de dados e como elas se conectam.
* **Uso Ideal**: Definição de tabelas de banco de dados, chaves primárias/estrangeiras e relacionamentos.
* **Elementos Comuns**: IDs, nomes, tipos de políticas, serviços e atribuições.

### 2.5 State Diagram (Diagrama de Estado)
Utilizado para representar a transição de estados dentro de um sistema ou componente.

---

## 3. Sintaxe e Ferramentas de Apoio
A criação de diagramas segue uma sintaxe lógica e simples:

* **Direcionamento**: O fluxo pode ser definido como `TD` (top-down / cima para baixo) ou `LR` (left-to-right / esquerda para direita).
* **Identificadores**: Cada nó possui um identificador único para evitar repetições e conflitos no fluxo.
* **Renderização**: O código é inserido em blocos Markdown utilizando três crases seguidas da palavra-chave `mermaid`.

### Mermaid Live Editor
É uma ferramenta gratuita que oferece:
* **Playground para Testes**: Visualização em tempo real do diagrama conforme o código é escrito.
* **Recurso de Correção**: Auxilia na identificação de erros de sintaxe.
* **Salvamento**: Permite criar uma conta para armazenar e organizar diversos diagramas.

---

## 4. Automação e Inteligência Artificial
A geração de diagramas Mermaid pode ser otimizada através de agentes de IA especializados, como o `MermaidDiagramGenerator`.

### Diretrizes de Automação
* **Consistência**: O agente deve manter a terminologia técnica entre português e inglês, seguindo o Feature Design Doc.
* **Qualidade Visual**: Priorizar labels curtas, evitar emojis e manter uma sintaxe limpa.
* **Escopo**: Recomenda-se a geração de 6 a 8 diagramas por projeto para manter o equilíbrio, evitando redundâncias.
* **Complexidade**: Diagramas com mais de 10 nós devem ser divididos; fluxos com mais de 8 etapas devem ser agrupados.

### Workflow do Agente de IA
1.  **Leitura e Extração**: Analisa o documento de design de funcionalidades.
2.  **Identificação**: Mapeia pontos arquiteturais, APIs públicas e cenários de erro.
3.  **Geração**: Cria os diagramas (sequência, flowchart, classes, etc.) em um único arquivo Markdown consolidado.
4.  **Autorrevisão**: Realiza uma fase de correção interna para garantir que o código Mermaid compile sem erros e reflita fielmente a lógica do sistema.

---

## Conclusão
O uso do Mermaid, especialmente quando aliado à automação por IA, transforma a documentação técnica de um fardo manual em um ativo dinâmico e sempre atualizado. Sua capacidade de viver dentro do repositório de código como texto puro garante que arquitetos e desenvolvedores tenham uma visão clara da estrutura e do comportamento do sistema sem a complexidade de ferramentas de design tradicionais.

### [Assista ao resumo em vídeo](https://github.com/user-attachments/assets/20ae3e90-dd30-47de-beec-7270953f49d7)
