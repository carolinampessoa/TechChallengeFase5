📌 **Tech Challenge – Fase 5**

Modelagem de Ameaças utilizando LLM Multimodal + STRIDE

🎯 **Objetivo**

Este projeto implementa um MVP de modelagem de ameaças automatizada a partir de diagramas de arquitetura de software em formato de imagem.
A solução utiliza um modelo multimodal (LLM) para interpretar semanticamente os componentes do diagrama e um motor de regras STRIDE para identificação de ameaças de segurança.

🧠 **Abordagem Técnica**

A arquitetura da solução segue o pipeline:
Imagem do Diagrama → LLM Multimodal → Extração Estruturada → STRIDE Engine → Relatório
Não há treinamento supervisionado.
O modelo de IA é utilizado como mecanismo de extração semântica, reduzindo custo computacional e complexidade de dataset rotulado.

🔍 **Dataset**

O dataset contém 5 diagramas de arquitetura de software, utilizados exclusivamente para validação experimental.
O objetivo não é treinamento, mas sim verificar:

* Capacidade de identificação de componentes
* Robustez frente a diferentes layouts
* Consistência da análise STRIDE

🛡 **STRIDE Engine**

Cada componente identificado é analisado conforme regras baseadas na metodologia STRIDE:
* Spoofing
* Tampering
* Repudiation
* Information Disclosure
* Denial of Service
* Elevation of Privilege

⚙ **Tecnologias Utilizadas**

* Python
* Google Colab
* OpenAI Multimodal Models
* Engenharia de Prompt
* STRIDE Threat Modeling

🧠 **Fluxo geral da solução**

O pipeline completo do sistema funciona da seguinte forma:

1️⃣ Upload do diagrama arquitetural  
2️⃣ Extração automática de componentes via LLM  
3️⃣ Normalização taxonômica dos elementos  
4️⃣ Aplicação do modelo STRIDE  
5️⃣ Enriquecimento das ameaças com explicações e contramedidas  
6️⃣ Geração automática de relatório técnico em PDF

📊 **Resultados**

A saída do sistema consiste em:
* Lista estruturada de componentes
* Ameaças STRIDE associadas
* Contramedidas sugeridas via LLM

🚀 **Conclusão**

Esse fluxo demonstra como **modelos de linguagem podem ser utilizados para automatizar atividades de Threat Modeling**, eliminando necessidade de treinamento customizado para MVPs, reduzindo esforço manual e aumentando a velocidade de análise de arquiteturas de software.
