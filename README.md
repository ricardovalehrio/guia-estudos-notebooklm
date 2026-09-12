# 🚀 Guia de Estudos: Como ser um Citizen Developer (Foco em Contabilidade e TI)

Bem-vindo ao meu caderno temático sobre **Citizen Development**, gerado a partir de estudos guiados por IA (NotebookLM). Este projeto documenta a minha jornada de aprendizado na intersecção entre regras de negócio contábeis/fiscais e o desenvolvimento de software.

## 🎯 Contexto e Objetivos

Sendo estudante de Ciências da Computação na Universidade Federal de Sergipe (UFS) e possuindo forte interface com Ciências Contábeis, minha vivência em rotinas administrativas — como rastreamento de notas fiscais, controle de suprimentos e fluxos de aprovação — deixou clara a necessidade de automatizar processos. 

O movimento *Citizen Developer* capacita profissionais que conhecem a fundo as regras de negócio a construírem suas próprias soluções utilizando ferramentas de Low-Code/No-Code (como n8n) integradas a linguagens como Python e bancos de dados SQL. 

**Meus objetivos com este caderno são:**
1. Compreender os fundamentos do Citizen Development e como ele transforma o setor fiscal e administrativo.
2. Mapear como ferramentas No-Code (n8n) podem ser integradas com scripts tradicionais (Python/Go) para automatizar o controle de notas fiscais e cotações.
3. Criar uma base de conhecimento (Glossário e Prompts) para revisões futuras e aplicação em projetos reais.

---

## 📚 Curadoria de Fontes

Para alimentar o NotebookLM e garantir um embasamento técnico (incluindo materiais audiovisuais), utilizei as seguintes fontes abertas:

1. **[Artigo Alura: Citizen developer - O que é, benefícios e como começar](https://www.alura.com.br/artigos/citizen-developer)** - *Texto base* para entender a definição corporativa, a diferença em relação a um Analista de Sistemas e os riscos do Shadow IT.
2. **[Vídeo YouTube: N8N para iniciantes - Criando sua Primeira AUTOMAÇÃO](https://www.youtube.com/watch?v=C0SDjqmctfU)** - *Fonte prática* para estruturar os tutoriais de automação de fluxo de trabalho no miniguia.
3. **[Vídeo YouTube: Citizen Developers - Who Are They And What Do They Do?](https://www.youtube.com/watch?v=2mADc-rlBX8)** - *Fonte conceitual* para consolidar a criação do glossário e entender o impacto nos negócios.
4. **[Zeev: Como se tornar um citizen developer?](https://zeev.it/blog/como-se-tornar-um-citizen-developer/)** - *Artigo de Negócios* detalhando a transição de um Analista de Negócios para um Desenvolvedor Cidadão, listando hard skills e soft skills necessárias.
5. **[Pipefy: O que é Citizen Automation e como funciona?](https://www.pipefy.com/pt-br/blog/o-que-e-citizen-automation/)** - *Guia prático* de automação cidadã com foco em fluxos de trabalho administrativos e de back-office.
6. **[Vídeo: Você já ouviu falar do Citizen Developer?](https://www.youtube.com/shorts/94S1fCjsm14)** - *Material audiovisual* discutindo a vantagem de capacitar profissionais contábeis em tecnologia em vez de ensinar regras de negócios complexas para programadores.
---

## 🛠️ Engenharia de Prompts e "Cicatrizes" (Troubleshooting)

Durante a interação com o NotebookLM sobre os documentos curados, testei diferentes abordagens para extrair o melhor conhecimento.

### Teste 1: O Conceito Geral
* **Prompt:** *"Com base nos documentos, resuma o que é um Citizen Developer e quais os riscos de não haver governança."*
* **Cicatriz (Dificuldade):** A IA retornou uma resposta muito genérica, focada apenas em TI, ignorando a parte de negócios.
* **Ajuste (Prompt Refinado):** *"Aja como um Diretor de Tecnologia. Com base no material do Gartner e do PMI, explique o papel do Citizen Developer no setor de contabilidade. Destaque 3 riscos de Shadow IT (TI invisível) caso um analista fiscal crie automações sem avisar a governança de TI."*
* **Resultado:** Resposta excelente, detalhando como a falta de documentação em rotinas fiscais pode gerar multas e problemas de auditoria.

### Teste 2: Aplicação Prática (Contabilidade + TI)
* **Prompt:** *"Como usar as ferramentas citadas nos textos para automatizar notas fiscais?"*
* **Cicatriz (Dificuldade):** A resposta veio em formato de texto corrido, difícil de transformar em um plano de ação, e misturou conceitos sem focar nas ferramentas.
* **Ajuste (Prompt Refinado):** *"Com base na documentação do n8n e no uso de Python, crie um fluxo de trabalho passo a passo (em bullet points) detalhando como um Citizen Developer pode automatizar a leitura de um XML de Nota Fiscal recebido por e-mail, extrair os dados e salvar em um banco de dados relacional PostgreSQL."*
* **Resultado:** A IA estruturou um pipeline perfeito: Trigger (Email n8n) -> Parser (Python/XML) -> Database Node (PostgreSQL), alinhando teoria à minha prática de banco de dados.

---

## 📖 Miniguia de Estudo (Entrega Final)

### 1. Resumo Estruturado do Assunto
O *Citizen Developer* não é um "programador amador", mas sim um especialista de negócios (ex: um assistente fiscal ou contador) que utiliza plataformas de desenvolvimento aprovadas pela TI corporativa para criar aplicativos e automações. 
* **O Problema:** A fila de demandas do departamento de TI é gigantesca. Tarefas menores, como "criar um alerta de escassez de material na obra" ou "cruzar uma fatura com um pedido de compra", raramente são priorizadas.
* **A Solução:** Utilizar ferramentas visuais (n8n, Zapier) ou linguagens de script (Python) para conectar APIs e automatizar essas conciliações, garantindo agilidade.
* **Governança:** É crucial evitar a *Shadow IT*. O desenvolvimento deve seguir boas práticas (versionamento no GitHub, uso de containers Docker) mesmo sendo feito pela área de negócios.

### 2. Glossário de Conceitos
* **Citizen Developer:** Usuário de negócios que cria capacidades de TI usando ferramentas prescritas e sancionadas pela organização.
* **Low-Code / No-Code (LCNC):** Plataformas que permitem criar softwares por meio de interfaces gráficas e arrastar-e-soltar, minimizando a necessidade de escrever código do zero.
* **Shadow IT:** Sistemas, softwares ou planilhas complexas usados dentro de uma empresa sem o conhecimento ou aprovação do departamento de TI (um risco grave para auditorias contábeis).
* **n8n:** Ferramenta de automação de fluxo de trabalho baseada em nós, que permite conectar diferentes APIs e serviços de forma visual.
* **Governança de TI:** Conjunto de regras e políticas que garantem que a tecnologia apoie os objetivos do negócio com segurança e conformidade.

### 3. Prompts Reutilizáveis para Revisão
Para futuras atualizações deste guia ou para estudos contínuos, posso utilizar os seguintes prompts no NotebookLM:

> 1. *"Com base nos meus documentos, gere um questionário de múltipla escolha com 5 perguntas difíceis sobre as diferenças entre um fluxo No-Code e o desenvolvimento tradicional."*
> 2. *"Atue como um auditor fiscal. Avalie o fluxo de automação de notas fiscais que criei e aponte possíveis falhas de segurança segundo a documentação de governança do PMI."*
> 3. *"Gere um mapa mental textual relacionando 'Ciências Contábeis', 'APIs', 'Python' e 'Citizen Development'."*

---
*Projeto desenvolvido como parte de um desafio prático de estudos em IA e Produtividade.*
