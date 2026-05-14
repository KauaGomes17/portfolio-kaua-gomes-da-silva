# 🏦 Sistema de Auditoria de Recursos Corporativos
 
## 📝 Descrição do Projeto
Este projeto consiste em uma ferramenta de análise financeira automatizada desenvolvida para consolidar orçamentos departamentais em estruturas corporativas complexas (Matrizes e Filiais). O sistema utiliza processamento recursivo para navegar por níveis hierárquicos de dados, permitindo o cálculo preciso de custos operacionais.

O diferencial técnico reside na implementação de um **Decorator de Auditoria**, que monitora em tempo real a execução das funções, registrando argumentos recebidos, tempos de processamento e metadados financeiros. É uma solução voltada para transparência e governança de dados em ambientes empresariais.

## 🛠️ Funcionalidades Principais
* **Cálculo Recursivo:** Navegação automática por dicionários aninhados representando diferentes níveis da empresa.
* **Decorator de Auditoria (@auditor):** Wrapper que intercepta chamadas de função para gerar logs de execução e performance.
* **Filtragem Dinâmica:** Capacidade de ignorar departamentos específicos durante a consolidação orçamental (usando `*args`).
* **Conversão de Moeda:** Suporte a taxas de câmbio dinâmicas para relatórios internacionais (usando `**kwargs`).

## 🚀 Tecnologias Utilizadas
* **Linguagem:** Python 3.x
* **Conceitos Avançados:** Decorators, Recursividade, Empacotamento/Desempacotamento de argumentos (`*args`, `**kwargs`).
* **Ferramentas:** Google Colab / Jupyter Notebook.

## 📊 Estrutura de Dados Exemplo
O sistema processa estruturas hierárquicas como o exemplo abaixo:
```python
empresa = {
    "Matriz": {
        "TI": {"Desenvolvimento": 80000, "Seguranca": 30000},
        "RH": {"Recrutamento": 20000}
    },
    "Filial_SP": {
        "Marketing": {"Publicidade": 25000}
    }
}

🔧 Como Executar
Certifique-se de ter o Python instalado ou utilize o Google Colab.

Clone este repositório:
git clone [https://github.com/seu-usuario/sistema-auditoria-corporativa.git](https://github.com/seu-usuario/sistema-auditoria-corporativa.git)

Abra o arquivo sistema_de_auditoria.ipynb no seu ambiente Jupyter.

Execute as células para visualizar os logs da auditoria e o resultado final do orçamento convertido.


Aqui está uma versão profissional do README estruturada especificamente para o seu projeto de Auditoria de Recursos Corporativos, seguindo as boas práticas de documentação para o GitHub.

Markdown
# 🏦 Sistema de Auditoria de Recursos Corporativos
 
## 📝 Descrição do Projeto
Este projeto consiste em uma ferramenta de análise financeira automatizada desenvolvida para consolidar orçamentos departamentais em estruturas corporativas complexas (Matrizes e Filiais). O sistema utiliza processamento recursivo para navegar por níveis hierárquicos de dados, permitindo o cálculo preciso de custos operacionais.

O diferencial técnico reside na implementação de um **Decorator de Auditoria**, que monitora em tempo real a execução das funções, registrando argumentos recebidos, tempos de processamento e metadados financeiros. É uma solução voltada para transparência e governança de dados em ambientes empresariais.

## 🛠️ Funcionalidades Principais
* **Cálculo Recursivo:** Navegação automática por dicionários aninhados representando diferentes níveis da empresa.
* **Decorator de Auditoria (@auditor):** Wrapper que intercepta chamadas de função para gerar logs de execução e performance.
* **Filtragem Dinâmica:** Capacidade de ignorar departamentos específicos durante a consolidação orçamental (usando `*args`).
* **Conversão de Moeda:** Suporte a taxas de câmbio dinâmicas para relatórios internacionais (usando `**kwargs`).

## 🚀 Tecnologias Utilizadas
* **Linguagem:** Python 3.x
* **Conceitos Avançados:** Decorators, Recursividade, Empacotamento/Desempacotamento de argumentos (`*args`, `**kwargs`).
* **Ferramentas:** Google Colab / Jupyter Notebook.

## 📊 Estrutura de Dados Exemplo
O sistema processa estruturas hierárquicas como o exemplo abaixo:
```python
empresa = {
    "Matriz": {
        "TI": {"Desenvolvimento": 80000, "Seguranca": 30000},
        "RH": {"Recrutamento": 20000}
    },
    "Filial_SP": {
        "Marketing": {"Publicidade": 25000}
    }
}
🔧 Como Executar
Certifique-se de ter o Python instalado ou utilize o Google Colab.

Clone este repositório:

Bash
git clone [https://github.com/seu-usuario/sistema-auditoria-corporativa.git](https://github.com/seu-usuario/sistema-auditoria-corporativa.git)
Abra o arquivo sistema_de_auditoria.ipynb no seu ambiente Jupyter.

Execute as células para visualizar os logs da auditoria e o resultado final do orçamento convertido.

📈 Resultados e Aprendizados
Logs Detalhados: O sistema gera um rastro de auditoria para cada chamada recursiva, facilitando o debug de grandes volumes de dados.

Performance: Implementação de monitoramento de tempo com precisão de microssegundos.

Flexibilidade: O uso de argumentos nomeados permite que a lógica de conversão de moeda seja injetada apenas quando necessário, sem quebrar a recursão base.

---
[Voltar ao início](https://github.com/KauaGomes17/portfolio-kaua-gomes-da-silva)
