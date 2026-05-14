# 🛡️ Algoritmo de Auditoria de Dados

## 📝 Descrição do Projeto
Este projeto consiste em um sistema em Python desenvolvido para automatizar processos de **compliance financeiro** e **auditoria de dados de vendas**. O script realiza a captura e o tratamento de dados de transações, calcula métricas operacionais e aplica regras de negócio rigorosas para identificar discrepâncias e mitigar riscos de segurança.

O sistema analisa os valores inseridos, calcula médias e valida se os registros estão em conformidade com políticas de segurança estabelecidas, disparando alertas de quarentena ou revisão manual caso identifique anomalias.

---

## 🚀 Funcionalidades
* **Tratamento e Conversão de Tipos:** Conversão explícita (*casting*) das entradas do usuário para ponto flutuante (`float`) para garantir a precisão dos cálculos financeiros.
* **Cálculo de Métrica:** Processamento da média aritmética das vendas registradas.
* **Detecção de Anomalias:** * **Quarentena:** Bloqueio preventivo se a média das vendas ultrapassar o limite de segurança configurado.
  * **Revisão Manual:** Identificação de picos de faturamento individuais que sejam **5 vezes maiores** que a média geral das vendas.
* **Gestão Dinâmica de Configurações:** Permite ao auditor alterar o limite de segurança em tempo de execução (`global`) caso uma transação legítima de alto valor seja detectada.

---

## 💻 Tecnologias Utilizadas
* **Linguagem:** Python 3.10+
* **Ambiente de Execução:** Terminal Python, Google Colab ou VS Code.

---

## 🔧 Como Executar o Projeto

### Pré-requisitos
* Ter o Python 3.10 ou superior instalado em sua máquina.

### Passo a Passo

1. **Clone este repositório:**
   ```bash
   git clone [https://github.com/seu-usuario/seu-repositorio.git](https://github.com/seu-usuario/seu-repositorio.git)
   cd seu-repositorio

2. **Execute o script de auditoria:**
   python projeto_algoritmo_de_auditoria_de_dados.py

3. **Interaja com o console:**

Insira os três valores de venda solicitados.

O sistema exibirá a média e os alertas correspondentes.

Caso alguma venda ultrapasse o limite de segurança, você terá a opção de atualizar o LIMITE_SEGURANCA diretamente no console.

📁 **Estrutura do Arquivo**
└── projeto_algoritmo_de_auditoria_de_dados.py  # Script principal de auditoria e compliance

---
[Voltar ao início](https://github.com/KauaGomes17/portfolio-kaua-gomes-da-silva)
