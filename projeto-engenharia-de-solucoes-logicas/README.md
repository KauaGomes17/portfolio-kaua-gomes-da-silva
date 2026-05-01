# 🎬 Sistema de Gestão Logística Inteligente

![License](https://img.shields.io/github/license/seu-usuario/logistica-ia?style=flat-square)
![Python Version](https://img.shields.io/badge/python-3.10%2B-blue?style=flat-square&logo=python)

## 📝 Descrição do Projeto

Este projeto consiste em um motor de roteirização e priorização de entregas desenvolvido para otimizar fluxos logísticos reais[cite: 1]. O sistema processa uma lista de entregas, calculando tempos estimados com base em distância e condições de tráfego, além de gerenciar prioridades dinâmicas (como clientes VIP ou urgências) para mitigar atrasos e falhas operacionais[cite: 1, 2, 4].

O motor foi estruturado para transformar problemas de tempo em soluções práticas, garantindo que a "janela de entrega" seja respeitada através de ajustes preditivos no tempo estimado[cite: 1, 2].

---

## ⚙️ Regras de Negócio e Algoritmo

O núcleo do sistema baseia-se em um fluxo lógico de decisão que processa cada entrega individualmente[cite: 2, 4]:

1.  **Cálculo Base:** O tempo estimado inicial é definido pela razão entre a distância e a velocidade média padrão (40 km/h)[cite: 2, 3].
2.  **Fator de Trânsito:** Caso o trânsito seja classificado como "alto", o sistema aplica um multiplicador de **1.5x** sobre o tempo estimado[cite: 2, 4].
3.  **Priorização:** Entregas marcadas como "prioritárias" ou de "clientes VIP" são automaticamente movidas para o topo da fila de execução[cite: 1, 4].
4.  **Validação de Janela:** O sistema confronta o tempo calculado com o prazo disponível, sinalizando status de "atrasada" caso o limite seja excedido[cite: 2, 4].

---

## 📊 Cenários de Teste

O sistema foi validado através de três estados principais[cite: 3]:

*   **Cenário A (Ideal):** Distância de 10km com trânsito normal e alta prioridade. Resultado: Tempo de 0.25h e prioridade no topo da lista[cite: 3].
*   **Cenário B (Limite):** Distância de 0km. Resultado: Entrega imediata (Tempo = 0)[cite: 3].
*   **Cenário C (Erro/Exceção):** Entrada de distância negativa (-5km). Resultado: O sistema identifica a inconsistência, emite erro e remove a entrega da fila para proteção dos dados[cite: 3].

---

## 🚀 Tecnologias Utilizadas

*   **Linguagem:** Python 3.10
*   **Lógica de Programação:** Estruturas de repetição (`enquanto houver entregas`) e condicionais aninhadas[cite: 2, 4].
*   **Versionamento:** Git para controle de alterações e documentação de melhorias.

---

## 🔧 Melhores Práticas e Robustez

Para elevar a maturidade do projeto (Cenário C), foram implementadas as seguintes melhorias[cite: 1]:

*   **Sanitização de Dados:** Bloqueio de valores negativos e caracteres de texto em campos numéricos[cite: 1].
*   **Tratamento de Exceções:** Mensagens de erro claras para falhas de entrada, evitando o colapso do sistema[cite: 1].
*   **Multifator de Urgência:** A prioridade agora considera múltiplos fatores (distância, tipo de cliente e urgência real)[cite: 1].

---

## 📂 Como Executar

1.  Clone o repositório.
2.  Certifique-se de ter o Python 3.10 instalado.
3.  Execute o script principal:
    ```bash
    python main.py
    ```

---
[Voltar ao topo](#-sistema-de-gestão-logística-inteligente)
