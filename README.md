# 🌐 Projeto: Mercado Híbrido de Previsão (FP&A Preditiva 2.0)

O **Mercado Híbrido de Previsão** é uma plataforma de inteligência financeira estratégica que une o poder do Machine Learning (ML) na previsão corporativa (FP&A - Financial Planning and Analysis) com a dinâmica de Mercados de Previsão (Prediction Markets). Nosso objetivo é transformar a incerteza em risco quantificável e decisões acionáveis.

---

## 🎯 Visão e Inovação

Este projeto visa superar as ferramentas de previsão legadas (Excel) e os mercados de previsão existentes (Ex: Kalshi) através de duas arquiteturas de valor:

### 1. Motor de Previsão Científica (ML Core)
Utilizamos ML para fornecer previsão de risco real (Monte Carlo) e **Auditoria Preditiva** (transparência da IA).

### 2. Contratos de Eventos Híbridos
A plataforma negocia probabilidade em três categorias de risco, garantindo um amplo **TAM (Total Addressable Market)**:
* **Estratégicos (FP&A):** Risco de MRR (Monthly Recurring Revenue) e LTV (Lifetime Value).
* **Operacionais:** Risco de Churn (Taxa de Cancelamento) e KPIs (Indicadores-Chave de Desempenho) de equipe.
* **Globais:** Eventos Macro/Financeiros.

---

## ✨ Funcionalidades Inovadoras (O MVP)

O Protótipo (MVP - Produto Mínimo Viável) será focado no nicho SaaS (Software as a Service) e demonstrará:

| Funcionalidade | Descrição Técnica | Valor para o Usuário |
| :--- | :--- | :--- |
| **AI Advisor (Consultor de IA)** | Sistema de NLP (Processamento de Linguagem Natural) que interpreta o *forecast*. | Gera **recomendações estratégicas acionáveis** (Ex: "Foque na retenção"). |
| **Simulação de Monte Carlo** | ML integrado para rodar milhares de simulações. | Quantifica o risco, informando a **probabilidade (%)** de atingir a meta (Lucro Líquido / DRE). |
| **Auditoria Preditiva** | Aplica o Fator de Ponderação de Drivers. | Demonstra **transparência** da IA, mostrando quais variáveis (Ex: Leads ou Preço) mais impactaram a previsão. |
| **Simulador de Cenários** | Interface UI com *sliders* para Drivers. | Recálculo **instantâneo** de todas as métricas financeiras (LTV, MRR, DRE) ao mover um Driver. |

---

## 🛠️ Stack Tecnológica (Fase 2 e 3)

| Componente | Ferramenta | Uso no Projeto |
| :--- | :--- | :--- |
| **Motor Preditivo (ML/Backend)** | **Python** | Linguagem principal para ML e lógica de negócio. |
| **Bibliotecas de ML** | **Prophet, NumPy, Pandas** | Modelagem de séries temporais, simulação de Monte Carlo e manipulação de dados. |
| **Frontend/Dashboard (MVP)** | **Dash (Plotly)** ou **Streamlit** (A ser decidido) | Construção da interface visual, *sliders* e gráficos de risco complexos. |
| **Integração Futura** | **API (Application Programming Interface)** | Meio de comunicação entre o Motor Preditivo (Python) e o Frontend/Plataformas externas. |

---

## 🚀 Como Executar o Projeto

### 1. Configuração do Ambiente

1.  Clone este repositório.
2.  Crie e ative um ambiente virtual (`venv`).
3.  Instale as dependências: `pip install pandas numpy prophet [outras libs para NLP/UI]`

### 2. Geração de Dados e Treinamento

Os scripts estão organizados em fases:

1.  `python gerar_dataset_sintetico.py`
    * *Ação:* Cria o arquivo `saas_historico_mvp.csv`.
2.  `python motor_preditivo.py`
    * *Ação:* Carrega o CSV, treina o modelo ML (Prophet com Regressores) e executa as funções de **Monte Carlo**, **LTV** e **DRE**.
3.  `python app_dashboard.py` (Fase 3)
    * *Ação:* Inicia a interface (Dash ou Streamlit) que consome os dados do Motor para visualização.

---

## 🗺️ Roadmap Modular (Próximas Fases)

* **Fase 3 (Protótipo):** Desenvolvimento do Dashboard interativo e integração da lógica do AI Advisor.
* **Fase 4 (Validação):** Testes de usabilidade e acurácia do modelo.
* **Fase 5 (Investimento):** Criação do Pitch Deck e busca por capital para a **Integração Enterprise (CRM/ERP)** e escalabilidade dos Mercados Globais.
