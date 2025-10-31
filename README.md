<img width="1024" height="585" alt="image" src="https://github.com/user-attachments/assets/01662548-3efa-4b90-bc53-624f40645584" />


# 🏭 Fábrica Inteligente: Manutenção Preditiva com Machine Learning

## Visão Geral do Projeto

Este projeto demonstra a construção de uma solução de Machine Learning de ponta a ponta para o problema de **manutenção preditiva industrial**. O objetivo é prever falhas em máquinas com base em dados de sensores em tempo real, permitindo que a equipe de manutenção atue de forma proativa, reduzindo custos com paradas inesperadas e otimizando a produção.

A solução final é um **dashboard interativo construído com Streamlit**, que serve tanto como uma ferramenta de Análise de Dados Gerencial (EDA) quanto como um sistema de monitoramento em tempo real (O "AI Machine Predicts Broken")

---
## Tecnologias Utilizadas

![Python](https://img.shields.io/badge/Python-3.12%2B-blue?logo=python&style=for-the-badge)
![Streamlit](https://img.shields.io/badge/Streamlit-Dashboard-FF4B4B?logo=streamlit&style=for-the-badge)
![XGBoost](https://img.shields.io/badge/XGBoost-Modelo_ML-006699?style=for-the-badge)
![SHAP](https://img.shields.io/badge/SHAP-Interpretabilidade-purple?style=for-the-badge)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-ML_Pipeline-orange?logo=scikit-learn&style=for-the-badge)
![Pandas](https://img.shields.io/badge/Pandas-Análise_de_Dados-150458?logo=pandas&style=for-the-badge)
![Plotly](https://img.shields.io/badge/Plotly-Visualização-blue?logo=plotly&style=for-the-badge)
![Jupyter](https://img.shields.io/badge/Jupyter-Laboratório_ML-F37626?logo=jupyter&style=for-the-badge)

A solução foi construída utilizando um ecossistema moderno de Data Science em Python, com foco em performance, interpretabilidade e entrega de valor de negócio.

| Categoria | Ferramenta | Utilização no Projeto |
| :--- | :--- | :--- |
| **Dashboard e Interface** | **Streamlit** | Para construir o dashboard interativo, servindo como a interface principal da solução para a gerência. |
| **Modelo de ML** | **XGBoost** | Como o algoritmo de Machine Learning principal, escolhido por sua alta performance e robustez em dados tabulares. |
| **Interpretabilidade (XAI)** | **SHAP** | Para a interpretabilidade do modelo ('Explainable AI'), permitindo a visualização do **porquê** o modelo toma cada decisão. |
| **Estrutura de ML** | **Scikit-learn** | Para criar o `Pipeline` de pré-processamento, padronizar as features (`StandardScaler`), codificar variáveis (`OneHotEncoder`) e avaliar o modelo. |
| **Análise de Dados** | **Pandas** | Para a manipulação, limpeza e preparação dos dados em todas as fases do projeto. |
| **Visualização de Dados** | **Plotly Express** | Para a criação dos gráficos interativos e gerenciais na fase de EDA do dashboard. |
| **Experimentação** | **Jupyter Notebook** | Como 'laboratório' para a experimentação, prototipação e validação do modelo de Machine Learning antes da produção. |
---

##  Demonstração do Dashboard

<img width="1024" height="1463" alt="image" src="https://github.com/user-attachments/assets/dbb2f35b-8a13-479e-a9db-03a438b17c9f" />

<img width="1031" height="1219" alt="image" src="https://github.com/user-attachments/assets/22ff098b-d6bb-4ffd-bb00-7f402021afbc" />

<img width="1009" height="1546" alt="image" src="https://github.com/user-attachments/assets/b31f3849-3764-4a04-9eec-143338b2f067" />

<img width="1007" height="1561" alt="image" src="https://github.com/user-attachments/assets/9c55c591-f68e-4b96-8005-1defe0686f5e" />

  ![aaohit](https://github.com/user-attachments/assets/492aeed7-29ee-40ac-a7c3-ba757f1ff0cf)

---


##  Principais Features

### 📊 Análise EDA Gerencial
* **Diagnóstico de Falhas:** Identificação visual dos tipos de falha mais comuns (HDF, PWF, etc.).
* **Análise de Causa Raiz:** Investigação profunda das condições operacionais (Torque, Rotação, Temperatura) que levam às falhas.
* **Análise de Desempenho:** Comparativo da taxa de falha entre máquinas de baixa, média e alta qualidade.
* **Análise de Desgaste:** Identificação do "ponto de virada" crítico (200 minutos) a partir do qual o risco de falha dispara.

### 🕵🏻‍♀️ AI Machine Predicts Broken
* **Modelo de Machine Learning:** Utilização do `XGBoost` treinado para classificar se uma máquina irá falhar ou não, com um **recall de 71%** no conjunto de teste.
* **Interpretabilidade com SHAP:** Análise do "cérebro" do modelo para entender quais sensores são mais importantes para as previsões.
* **Monitoramento em Tempo Real:** Uma interface interativa onde é possível selecionar uma máquina e receber um diagnóstico instantâneo do risco de falha.

---


## ⚙️ Como Executar Localmente

1.  **Clone o repositório:**
    ```bash
    git clone [https://github.com/seu-usuario/projeto-fabrica-inteligente.git](https://github.com/seu-usuario/projeto-fabrica-inteligente.git)
    cd projeto-fabrica-inteligente
    ```

2.  **Crie e ative o ambiente virtual:**
    ```bash
    python -m venv .venv
    .\.venv\Scripts\Activate
    ```

3.  **Instale as dependências:**
    ```bash
    pip install -r requirements.txt
    ```

4.  **Execute o dashboard Streamlit:**
    ```bash
    streamlit run dashboard.py
    ```

---

## 📁 Estrutura do Projeto

O projeto está organizado de forma modular para garantir clareza e reprodutibilidade, seguindo as melhores práticas da indústria:

* 📁 projeto-fabrica-inteligente
*  |---📁 dados |---📄 `predictive_maintenance.csv`: O dataset utilizado
*  |---📁 notebooks |---📄 `ml_experiments.ipynb`: Notebook com todo o processo de treino do modelo de ML
*  |---📁 Scripts |---📄 `dashboard.py`: Script da dashboard Streamlit 📄 `modelo_fabrica_inteligente.joblib`: Arquivo do modelo treinado
*  |---📄 `requirements.txt`: Lista de dependências do projeto 
*  |---📄 `README.md`: Este arquivo de documentação
*  |---📄 `.gitignore`: Arquivos e pastas a serem ignorados pelo Git


---

## 👨‍💻 Autor
**Marcelo Kudo**

## 💬 Sobre mim

**Engenheiro de Machine Learning & Especialista em Automação Industrial** 💡 **Foco:** IIoT | Análise de Dados | IA Industrial  

Profissional com **+18 anos de experiência em tecnologia** unindo **Automação Industrial**, **Análise de Dados** e **Inteligência Artificial**, aplicando tecnologia para otimizar processos industriais.  
Desenvolvo **modelos de Machine Learning** voltados à **manutenção preditiva** e **otimização de desempenho**, com foco em **integração direta com sistemas de controle**.

---

### ⚙️ Competências Técnicas
- 🧠 **Machine Learning:** TensorFlow, PyTorch, Keras  
- 🐍 **Programação:** Python (Pandas, NumPy), SQL  
- 📊 **Análise e Visualização:** Power BI, Dashboards de KPI’s  
- 🏭 **Automação & IIoT:** CLPs, IHMs, Edge AI, Rockwell, Mitsubishi, Schneider, além de Edge AI e sistemas de visão embarcada.

---

[comment]: <> (Link para o LinkedIn)
[<img align="left" alt="Marcelo Kudo | LinkedIn" width="24px" src="https://www.vectorlogo.zone/logos/linkedin/linkedin-icon.svg" />][linkedin]

[comment]: <> (Link para o GitHub)
[<img align="left" alt="Marcelo Kudo | GitHub" width="24px" src="https://www.vectorlogo.zone/logos/github/github-tile.svg" />][github]

[linkedin]: https://www.linkedin.com/in/[SEU_LINKEDIN_AQUI]
[github]: https://github.com/[SEU_USUARIO_DO_GITHUB]
