# 🚚 Sistema Integrado de Logística e Gestão de Pagamentos

![Python Version](https://img.shields.io/badge/python-3.10%2B-blue?style=flat-square)
![Status](https://img.shields.io/badge/status-em%20desenvolvimento-green?style=flat-square)

## 📝 Descrição do Projeto

Este projeto combina inteligência logística e processamento financeiro para otimizar operações de entrega[cite: 1, 5]. O sistema é capaz de calcular rotas e tempos de chegada baseados em condições de tráfego, ao mesmo tempo que gerencia a finalização da venda através de um motor de "Pagamento Suficiente", que valida transações e calcula a distribuição otimizada de cédulas para troco[cite: 2, 5, 6].

---

## ⚙️ Módulos do Sistema

### 1. Motor de Logística e Roteirização
O algoritmo de logística processa uma fila de entregas utilizando variáveis em tempo real[cite: 2, 4]:
*   **Cálculo de Tempo:** A estimativa base segue a fórmula $\text{tempo} = \text{distância} / 40$[cite: 2, 3].
*   **Ajuste Dinâmico de Tráfego:** Se o trânsito estiver alto, o tempo estimado recebe um acréscimo de 50% (multiplicador 1.5)[cite: 2, 4].
*   **Gestão de Prioridades:** Clientes VIP ou pedidos com alta urgência são automaticamente movidos para o topo da lista de execução[cite: 1, 2, 4].
*   **Status de Atraso:** O sistema valida se o tempo estimado ultrapassa a janela de horário disponível, marcando o status como "atrasada" quando necessário[cite: 2, 4].

### 2. Motor Financeiro (Troco Otimizado)
Responsável por garantir a integridade da transação no ato da entrega[cite: 5, 6]:
*   **Validação de Pagamento:** Compara o valor pago com o valor da compra para autorizar a transação[cite: 5].
*   **Cálculo de Troco:** Determina o valor residual a ser devolvido[cite: 5].
*   **Decomposição de Cédulas:** Utiliza lógica de divisão inteira e resto para calcular a menor quantidade possível de notas (100, 50, 10, 5 e 1)[cite: 5, 7].

---

## 📊 Cenários de Execução Logística

| Cenário | Entrada | Comportamento do Sistema |
| :--- | :--- | :--- |
| **A (Ideal)** | 10km, Trânsito Normal, Prioridade Alta | Calcula 0.25h e prioriza no topo da lista[cite: 3]. |
| **B (Limite)** | 0km | Processa como entrega imediata (tempo zero)[cite: 3]. |
| **C (Erro)** | Distância Negativa (-5km) | Identifica inconsistência, remove a entrega e emite alerta[cite: 1, 3]. |

---

## 🛠️ Detalhes da Implementação

### Lógica de Decomposição de Notas
A função `decompor_notas` segue o método sucessivo para garantir eficiência no caixa[cite: 5, 7]:
*   **Nota 100:** `notas100 = troco // 100`[cite: 5].
*   **Resto:** `troco = troco % 100`[cite: 5].
*   Repete-se o processo para as demais cédulas até a unidade[cite: 7].

### Boas Práticas Adotadas
*   **Sanitização de Entradas:** Bloqueio de valores negativos e validação de tipos (impedindo texto em campos numéricos)[cite: 1].
*   **Mensagens de Erro Claras:** Substituição de falhas de sistema por orientações ao usuário[cite: 1].
*   **Arquitetura Top-Down:** Refinamento sucessivo da lógica de pagamento para facilitar a manutenção[cite: 6].

---

## 🚀 Como Executar

1. Clone o repositório.
2. Execute o módulo principal:
   ```bash
   python main.py

   ---
[Voltar ao início](https://github.com/KauaGomes17/portifolio-kaua-gomes-da-silva)
