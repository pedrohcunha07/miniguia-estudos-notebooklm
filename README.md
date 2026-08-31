

readme_content = """# Caderno Temático: Engenharia de Requisitos com NotebookLM

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

#### **Interação 2: Prompt Estruturado (Iteração Bem-Sucedida)**
* **Prompt Utilizado:**
  ```text
  Com base estritamente nos documentos carregados, atue como um Engenheiro de Software Sênior e elabore um resumo em tabela comparando Requisitos Funcionais (RF), Requisitos Não-Funcionais (RNF) e Regras de Negócio (RN). Inclua para cada um: definição, 2 exemplos práticos de um sistema e-commerce e os critérios de validação.
