# 🚀 Logic & Environment Suite: Simulação e Análise Urbanas

## 📝 Descrição do Projeto
Este repositório contém uma suíte de ferramentas desenvolvidas em Python voltadas para a simulação de sistemas de decisão e análise técnica de dados de microclima. O projeto utiliza estruturas de dados multidimensionais e lógica de estados para modelar situações do mundo real, desde a segurança em ambientes domésticos até o monitoramento da qualidade de vida em centros urbanos.

Os algoritmos foram projetados para demonstrar o uso de estruturas de controle avançadas, como loops de simulação e processamento de matrizes, oferecendo diagnósticos detalhados sobre variáveis críticas de conforto e segurança.

## 📂 Estrutura do Repositório

### 1. Sistema de Navegação e Evacuação (`navegação_evacuação_espacial.py`)
Um simulador lógico que modela a movimentação de um indivíduo em um ambiente em crise:
* **Máquina de Estados:** Gerencia a transição entre locais como quartos, sala, cozinha e saída.
* **Gestão de Energia:** Cada movimento e obstáculo (como fogo leve ou escadas) consome pontos de energia, exigindo planejamento estratégico para a sobrevivência.
* **Sistema de Inventário:** Inclui a busca e o uso de itens (chaves) para desbloquear caminhos trancados durante a rota de fuga.

### 2. Algoritmo de Análise de Microclima (`algoritmo_microclima_local.py`)
Uma ferramenta de processamento de dados ambientais focada em métricas de saúde e bem-estar urbano:
* **Classificação de Qualidade do Ar (IQA):** Utiliza o padrão oficial para categorizar o ar entre "Boa", "Moderada", "Ruim", "Muito Ruim" ou "Péssima" via lógica `match-case`.
* **Cálculo de Conforto Urbano:** Aplica uma fórmula matemática que gera uma nota de 0 a 10, penalizando extremos de temperatura e umidade relativa.
* **Análise de Localidades:** Processa simultaneamente dados de múltiplos pontos geográficos, como Terminais e Shoppings.

## 🚀 Tecnologias Utilizadas
* **Linguagem:** Python 3.10+
* **Ambiente:** Google Colab / Jupyter Notebook
* **Lógica:** Programação baseada em eventos, análise de dados e estruturas condicionais.

## 🔧 Como Executar
1. Clone o repositório para sua máquina local.
2. Certifique-se de ter o Python 3 instalado.
3. Para iniciar a simulação de segurança, execute:
   ```bash
   python navegação_evacuação_espacial.py
4. Para gerar o relatório de dados ambientais, execute:
   python algoritmo_microclima_local.py

📊 Aprendizados Aplicados
Desenvolvimento de Algoritmos: Criação de lógica de progressão e retrocesso em listas de estados.

Matemática Aplicada: Implementação de cálculos de penalização para índices de conforto urbano.

Tratamento de Dados: Manipulação de listas de listas para representação de datasets ambientais.

[Voltar ao início](https://github.com/KauaGomes17/portifolio-kaua-gomes-da-silva)
