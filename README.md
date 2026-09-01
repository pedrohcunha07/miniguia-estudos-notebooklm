# Caderno Temático: Engenharia de Requisitos com NotebookLM

**Projeto prático desenvolvido para o desafio de projeto da [DIO (Digital Innovation One)](https://www.dio.me/).**  
Este repositório é um caderno de estudos interativo sobre **Engenharia de Requisitos em Software**, construído utilizando o **Google NotebookLM** como ferramenta de aprendizagem ativa, curadoria de conhecimento e assistência orientada por Inteligência Artificial.

---

## 1. Contexto e Objetivos

### Contexto do Tema
A **Engenharia de Requisitos (ER)** é a espinha dorsal do desenvolvimento de software de alta qualidade. Grande parte dos insucessos em projetos de tecnologia decorre de falhas no levantamento, na documentação, na validação ou na gestão de mudanças de requisitos. 

Com o avanço da Inteligência Artificial Generativa, torna-se essencial aprender a sintetizar grandes volumes de documentação técnica, livros, normas (como a ISO/IEC/IEEE 29148) e frameworks ágeis utilizando assistentes inteligentes como o **NotebookLM**.

### Objetivos de Estudo
* **Compreender os Fundamentos:** Mapear os pilares essenciais da Engenharia de Requisitos (Elicitação, Análise, Especificação, Validação e Gestão).
* **Explorar IA na Prática:** Testar a capacidade do NotebookLM em sintetizar fontes abertas técnicas sem alucinações.
* **Construir um Guia Prático:** Gerar um material de consulta rápida e reutilizável contendo resumos, glossário e biblioteca de prompts otimizados.

---

## 2. Curadoria de Fontes

Para alimentar a base de conhecimento no NotebookLM, foram selecionadas **4 fontes abertas (PDFs/Artigos técnicos)** de alta confiabilidade no domínio de Engenharia de Software:

| # | Fonte / Título | Tipo de Documento | Foco / Conteúdo |
|---|---|---|---|
| 1 | [Engenharia de Requisitos - (Gran Cursos Online)](https://blog.grancursosonline.com.br/engenharia-de-requisitos/) | Página Web/Blog | Introdução e conteúdo geral/superficial sobre o que é cobrado em concursos de TI/ER |
| 2 | [Introdução a Engenharia de Requisitos - (Dev Media)](https://www.devmedia.com.br/introducao-a-engenharia-de-requisitos/8034) | Página Web/Blog | Introdução de conteúdo sobre ER, até gerência e qualidade de requisitos |
| 3 | [Engenharia de Requisitos: Um Resumo Rumo à Prática - (Brasil Acadêmico)](https://blog.brasilacademico.com/2026/03/engenharia-de-requisitos-um-resumo-rumo.html) | Página Web/Blog | Resumo de ER, com metodologia semelhante á conteúdo de aula com fontes de professores |
| 4 | [Engenharia de Requisitos: o que é, como funciona e quais fases existem - (QueroBolsa)](https://querobolsa.com.br/revista/engenharia-de-requisitos) | Página Web/Blo | Introdução a engenharia de requisitos e suas fases |

---

## 3. Engenharia de Prompts e "Cicatrizes" (Troubleshooting)

Nesta seção estão documentadas as interações com o NotebookLM, demonstrando o raciocínio por trás do refinamento das perguntas e como as limitações da IA foram superadas.

### Testes de Prompts e Evolução

#### **Interação 1: Tentativa Genérica**
* **Prompt Utilizado:** `"Explique o que é engenharia de requisitos."`
* **Resposta Obtida:** Resposta vaga e excessivamente teórica, abordando tópicos gerais de TI sem profundidade.
* **Refinamento:** Aplicou-se técnica de *Role-Playing* e restrição de escopo com base nos documentos enviados.

#### **Interação 2: Tentativa Genérica 2**
* **Prompt Utilizado:** `"Explique a diferença entre requisitos funcionais e não funcionais."`
* **Resposta Obtida:** Resposta vaga, mas com leve aprofundamento no conteúdo através de tabelas.
* **Refinamento:** Aplicou-se escopo com base nos documentos enviados.

#### **Interação 3: Prompt Estruturado (Iteração Bem-Sucedida)**
* **Prompt Utilizado:**
  ```text
  Com base estritamente nos documentos carregados, atue como um Engenheiro de Software Sênior e elabore um resumo em tabela comparando Requisitos Funcionais (RF), Requisitos Não-Funcionais (RNF) e Regras de Negócio (RN). Inclua para cada um: definição, 2 exemplos práticos de um sistema e-commerce e os critérios de validação.

* **Resposta Obtida:** Resposta mais aprofundada e coesa, com tabelas explicativas e visão arquitetural.

## Resumo

A Engenharia de Requisitos (ER) sistematiza as atividades de descoberta, análise, especificação, validação e gerência das necessidades em sistemas de software. Suas etapas dividem-se em Produção (levantamento, registro, verificação e validação) e Gerência (controle de mudanças, configuração, rastreabilidade e qualidade);
Na Elicitação, descobrem-se as necessidades por técnicas como entrevistas, workshops (JAD), prototipação, análise documental e observação

A Especificação formaliza esses requisitos de forma correta, completa, clara, consistente, modificável, verificável, priorizada e rastreável. A Verificação garante que os requisitos foram descritos corretamente, enquanto a Validação assegura que o produto atende às necessidades reais.

Requisitos dividem-se em Funcionais (ações que o sistema executa) e Não Funcionais (atributos de qualidade e restrições técnicas). Existem ainda os requisitos de Negócio (metas corporativas de alto nível) e os de Domínio (regras e fórmulas do setor específico).

A Rastreabilidade mapeia o caminho de cada requisito desde a sua origem até a implementação no código e nos testes. A priorização pelo método MoSCoW separa o escopo em quatro categorias hierárquicas essenciais (Must, Should, Could, Won't). A Justificativa Lean define o MVP focado no aprendizado rápido, combatendo desperdícios de esforço, como o desenvolvimento de funcionalidades extras.

## Glossário de Conceitos

* **Engenharia de Requisitos (ER):** Disciplina que engloba as atividades sistemáticas e repetíveis destinadas a descobrir, analisar, documentar, validar e gerenciar necessidades e restrições de um sistema.
  
* **Requisitos Funcionais (RF):** Descrevem as funcionalidades, comportamentos e serviços diretos que o sistema oferecerá ao usuário.
  
* **Requisitos Não Funcionais (RNF):** Definem como o sistema deve se comportar, determinando restrições técnicas e atributos de qualidade (como usabilidade, segurança, desempenho e disponibilidade).
  
* **Requisitos de Negócio:** Especificações de alto nível que justificam o projeto, explicitando o "porquê" de sua criação.
  
* **Requisitos de Domínio:** Características, restrições e regras de cálculo específicas do setor ou ambiente de negócio no qual o software se aplica.
  
* **Elicitação (ou Levantamento):** Processo social e técnico para extrair, descobrir e refinar requisitos junto aos stakeholders.
  
* **Verificação:** Atividade realizada pela equipe técnica para conferir se as especificações foram escritas de forma adequada, consistente e sem ambiguidades ("estamos construindo o produto corretamente?").
  
* **Validação:** Atividade realizada junto aos stakeholders para obter o aceite formal e assegurar que as especificações refletem suas necessidades reais ("estamos construindo o produto certo?").
  
* **Rastreabilidade:** Capacidade de acompanhar a história de um requisito em nível horizontal ou vertical, desde sua origem até sua implementação em artefatos de código ou testes.
  
* **MoSCoW:** Técnica de priorização de requisitos que os classifica em Must have (essencial), Should have (importante), Could have (desejável) e Won't have (descartado na versão atual).
  
* **Produto Mínimo Viável (MVP):** Versão enxuta do produto contendo apenas as funcionalidades estritamente necessárias para entregar a proposta de valor central e validar hipóteses de mercado com menor esforço de desenvolvimento.
  
* **Justificativa Lean (Lean Business Case):** Enquadramento de uma iniciativa de negócio sob condições de incerteza, enxergando-a como uma hipótese testável cujos resultados são medidos iterativamente por indicadores.
 
* **Desperdício (Muda):** No contexto de desenvolvimento de software, é todo esforço empregado que não gera valor ou aprendizado imediato ao cliente, tendo as "funcionalidades extras" como seu exemplo mais crítico.
  
* **História de Usuário (User Story):** Unidade de trabalho ágil e leve que descreve um recurso de forma não técnica sob a perspectiva do usuário final.
  
* **Estrutura-se com base nos 3 Cs:** Cartão, Conversação e Confirmação.
  
* **INVEST:** Acrônimo que norteia os critérios de qualidade para a redação de histórias de usuário (Independent, Negotiable, Valuable, Estimable, Small, Testable).
  
* **Baseline:** Marco de desenvolvimento em que um conjunto de itens de configuração (especificações e diagramas) é estabilizado e colocado sob controle formal de mudanças.
