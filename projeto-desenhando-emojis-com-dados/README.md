# 🐍 Desafios de Estruturas de Dados em Python

## 📝 Descrição do Projeto
Este repositório reúne a resolução de três desafios práticos de manipulação de dados em Python. O objetivo principal é demonstrar o domínio sobre **estruturas de dados aninhadas** (dicionários, listas e tuplas) e a aplicação de **laços de repetição encadeados em múltiplos níveis** para processamento de informações.

Cada desafio aborda um cenário real de desenvolvimento:
1. **Desafio 1 (`desafio_1.py`)**: Manipulação de matrizes de pixels para edição de imagens.
2. **Desafio 2 (`desafio_2.py`)**: Processamento de sinais através de transposição de matrizes.
3. **Desafio 3 (`desafio_3.py`)**: Organização e exibição de metadados em sistemas de mídia.

---

## 🚀 Tecnologias Utilizadas
* **Linguagem:** Python 3.10 ou superior
* **Ambiente de Desenvolvimento:** Google Colab / Jupyter Notebook

---

## 📂 Detalhamento dos Desafios

### 🖼️ Desafio 1: Processamento de Imagem (Grade de Pixels)
Simulação de manipulação de uma matriz 5x5 que representa um emoji. O código aplica um efeito de "sombra" diminuindo o brilho de pixels amarelos específicos pela metade.

* **Conceito-chave:** Imutabilidade de tuplas (criação de novos objetos RGB) e filtragem condicional dentro de matrizes.
* **Complexidade:** 3 níveis de laços `for` (Dicionário → Linhas da Grade → Pixels).

### 🎵 Desafio 2: Transposição de Matrizes Musicais
Algoritmo que percorre uma biblioteca de frequências sonoras e realiza a transposição matemática de matrizes 2x2.

* **Conceito-chave:** Inversão de índices de linhas e colunas ($A_{i,j} = A_{j,i}$) e compreensão de listas para reconstrução de dados.
* **Complexidade:** 3 níveis de laços `for` (Lista de Toques → Dicionário de Frequências → Índices da Matriz).

### 🎬 Desafio 3: Playlist Visual com Metadados
Simulador de gerenciamento de álbuns e frames visuais. O script executa reordenação dinâmica de listas e exibição formatada com desempacotamento de dados.

* **Conceito-chave:** Manipulação de listas com os métodos `.pop()` e `.insert()`, e desempacotamento de tuplas aninhadas diretamente no laço de repetição.
* **Complexidade:** 3 níveis de laços `for` (Chaves do Dicionário → Álbuns → Frames).

---

## 📁 Estrutura do Repositório
```text
├── desafio_1.py       # Algoritmo de sombreamento de grade de pixels
├── desafio_2.py       # Algoritmo de transposição de matrizes musicais
├── desafio_3.py       # Gerenciador de metadados de playlists visuais
└── README.md          # Documentação do projeto

🔧 Como Executar os Scripts
Pré-requisitos
Python 3.10+ instalado em seu computador.

Passo a Passo
1. Clone este repositório:
git clone [https://github.com/seu-usuario/seu-repositorio.git](https://github.com/seu-usuario/seu-repositorio.git)
cd seu-repositorio

2. Execute os desafios individualmente:
python desafio_1.py
python desafio_2.py
python desafio_3.py

---
[Voltar ao início](https://github.com/KauaGomes17/portfolio-kaua-gomes-da-silva)
