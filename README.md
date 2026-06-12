# miniguia-estudos-notebooklm

Markdown
# 📘 Miniguia de Estudos: DevSecOps com NotebookLM

Bem-vindo ao repositório do meu projeto prático desenvolvido para o desafio da **Digital Innovation One (DIO)**. O objetivo deste projeto é explorar o uso da Inteligência Artificial (especificamente o NotebookLM do Google) como uma ferramenta de aprendizagem ativa, estruturando um caderno temático de alto nível técnico.

---

## 🎯 Contexto e Objetivos

No cenário atual de desenvolvimento de software, a velocidade de entrega não pode atropelar a segurança. Este caderno temático aborda a cultura e as práticas de **DevSecOps**, que consistem na integração de testes e validações de segurança desde o início do ciclo de desenvolvimento (abordagem *Shift-Left*), e não apenas no final.

### Objetivos de Estudo:
* Compreender os pilares da cultura DevSecOps e a diferença para o DevOps tradicional.
* Identificar as principais ferramentas e etapas de análise (SAST, DAST, SCA) em um pipeline CI/CD.
* Criar uma base de conhecimento sólida para aplicar práticas de segurança em projetos de infraestrutura e desenvolvimento.

---

## 📚 Curadoria de Fontes

Para alimentar o NotebookLM e garantir respostas precisas e embasadas, foram selecionadas as seguintes fontes públicas e de alta relevância técnica:

1. **OWASP Top 10 (Current Edition)** - O guia definitivo com as principais vulnerabilidades de segurança em aplicações web.
2. **CISA (Cybersecurity and Infrastructure Security Agency) - DevSecOps Basics** - Documentação governamental sobre a mentalidade e segurança em pipelines automatizados.
3. **Red Hat Guide: What is DevSecOps?** - Artigo técnico detalhando a integração de segurança em contêineres e automação.
4. **Google Cloud Architecture Framework: Security** - Boas práticas de gerenciamento de identidade, acessos e conformidade em ambientes Cloud.

---

## 🧠 Engenharia de Prompts e "Cicatrizes" (Troubleshooting)

Documentação do processo de iteração com a IA para extrair os melhores insights das fontes fornecidas.

### Teste de Prompt 1: Abordagem Direta (Genérica)
* **Prompt:** *O que é DevSecOps e como aplico no CI/CD?*
* **Resultado:** A IA trouxe uma resposta genérica, explicando o conceito básico, mas sem detalhar as ferramentas ou o momento exato de cada validação no pipeline.
* **Problema:** Resposta superficial, parecida com uma busca comum do Google.

### Teste de Prompt 2: Abordagem Estruturada e Contextualizada (Refinada)
* **Prompt:** *Com base nas fontes fornecidas (OWASP e CISA), atue como um Engenheiro de Segurança Sênior. Explique a diferença prática entre as análises SAST, DAST e SCA. Crie uma tabela indicando em qual fase do pipeline CI/CD (Commit, Build, Test, Deploy) cada uma deve ser executada e por quê.*
* **Resultado:** Resposta excelente. A IA mapeou o SAST no Commit/Build (análise de código estático), o SCA no Build (varredura de dependências/bibliotecas) e o DAST no Test/Deploy (teste em ambiente de execução), justificando com base nos guias anexados.
* **Lição Aprendida:** Dar um papel à IA (Engenheiro Sênior) e delimitar o escopo com base nas fontes melhora drasticamente a profundidade técnica do retorno.

---

## 📖 Miniguia de Estudo (Entrega Final)

### 1. Resumo Estruturado do Assunto

O **DevSecOps** promove a ideia de que a segurança é responsabilidade de todos no time, e não um gargalo final controlado por uma equipe isolada. 

* **Shift-Left:** Significa mover os testes de segurança para o início do ciclo de desenvolvimento. Encontrar uma vulnerabilidade na fase de código custa significativamente menos do que corrigi-la em produção.
* **Automação de Testes:** Para não desacelerar as entregas, as validações devem ser automatizadas dentro do pipeline:
  * **SAST (Static Application Security Testing):** Analisa o código-fonte antes de ser executado à procura de padrões inseguros (ex: SQL Injection, hardcoded credentials).
  * **SCA (Software Composition Analysis):** Varre as dependências e bibliotecas de terceiros utilizadas no projeto em busca de vulnerabilidades conhecidas (CVEs).
  * **DAST (Dynamic Application Security Testing):** Ataca a aplicação em tempo de execução (geralmente em ambiente de homologação) para encontrar falhas ativas.

### 2. Glossário de Conceitos-Chave

| Termo | Definição |
| :--- | :--- |
| **Shift-Left** | Prática de antecipar testes (especialmente de segurança e qualidade) para as fases iniciais do desenvolvimento. |
| **CI/CD** | Continuous Integration / Continuous Deployment. Automação do processo de integrar código, testar e implantar em produção. |
| **Pipeline** | O fluxo automatizado de passos que o código percorre desde o commit do desenvolvedor até o ambiente de produção. |
| **CVE** | *Common Vulnerabilities and Exposures*. Um dicionário público de falhas de segurança de conhecimento comum. |
| **Hardcoded** | Dados sensíveis (como senhas e chaves de API) escritos diretamente no código-fonte, o que gera alto risco de exposição. |

### 3. Prompts Reutilizáveis para Revisões Futuras

Salve estes prompts no seu NotebookLM para revisar ou expandir o conhecimento deste caderno:

* > *"Atue como um especialista em segurança de aplicações. Revise o conceito de Shift-Left contido nos documentos e gere 3 cenários práticos de como desenvolvedores podem aplicar isso no dia a dia sem perder produtividade."*
* > *"Com base no guia do OWASP fornecido, quais são as 3 principais vulnerabilidades que podem ser mitigadas utilizando exclusivamente ferramentas de SAST no pipeline? Explique a lógica."*
* > *"Gere um questionário de 5 perguntas de múltipla escolha com gabarito comentado para testar meus conhecimentos sobre a diferença entre SAST e DAST."*

---

## 🛠️ Tecnologias e Ferramentas Utilizadas
* **Google NotebookLM** (Curadoria, análise e geração de insights com IA)
* **GitHub** (Hospedagem e documentação do portfólio)
* **Markdown** (Formatação do guia de estudos)

---
Feito com 💻 por @Avelinebr
