# Megaline – Análise de Planos Pré-Pagos

Este projeto analisa dados da **Megaline**, empresa de telecomunicações, para determinar qual dos planos pré-pagos (Surf ou Ultimate) gera mais receita e entender o comportamento dos clientes.

---

## 🧪 Objetivo

Avaliar o comportamento dos clientes de diferentes planos pré-pagos e regiões, analisando chamadas, mensagens e uso de internet, para:

- Determinar qual plano gera mais receita média
- Identificar padrões de consumo por tipo de serviço
- Testar hipóteses sobre diferenças entre planos e regiões

---

## 🔍 Descrição do Projeto

O projeto está dividido em cinco etapas principais:

1. **Etapa 1 – Exploração de Dados:**  
   Abrir e inspecionar os arquivos CSV (`users`, `calls`, `messages`, `internet`, `plans`) para entender a estrutura e qualidade dos dados.

2. **Etapa 2 – Preparação dos Dados:**  
   - Conversão de tipos de dados  
   - Correção de erros e inconsistências  
   - Cálculo mensal por usuário:  
     - Número de chamadas e minutos usados  
     - Número de mensagens enviadas  
     - Volume de dados utilizado  
     - Receita mensal por usuário considerando limites do plano e cobranças adicionais

3. **Etapa 3 – Análise Exploratória:**  
   - Estatísticas descritivas (média, variância, desvio padrão)  
   - Histogramas de uso e receita  
   - Comparação entre planos Surf e Ultimate

4. **Etapa 4 – Teste de Hipóteses:**  
   - Comparar receitas médias entre planos  
   - Comparar receitas médias entre regiões (ex.: NY-NJ vs outras)  
   - Formular hipóteses nulas e alternativas  
   - Definir critério de decisão e valores alfa

5. **Etapa 5 – Conclusão:**  
   - Síntese dos principais resultados  
   - Recomendação sobre qual plano gera mais receita  
   - Insights sobre padrões de consumo

---

## 🚀 Tecnologias Utilizadas

- Python 3.11  
- Pandas, NumPy, Matplotlib, Seaborn  
- Jupyter Notebook  

> Bibliotecas adicionais estão listadas no `requirements.txt`.

---

## 📂 Dataset

O projeto utiliza cinco arquivos CSV contendo dados de 500 clientes:

| Arquivo | Conteúdo |
|---------|----------|
| `megaline_users.csv` | Informações do usuário: ID, nome, idade, cidade, plano, datas de registro e cancelamento |
| `megaline_calls.csv` | Chamadas: ID, data, duração (minutos), ID do usuário |
| `megaline_messages.csv` | Mensagens de texto: ID, data, ID do usuário |
| `megaline_internet.csv` | Sessões de internet: ID, volume usado (MB), data, ID do usuário |
| `megaline_plans.csv` | Planos disponíveis: nome, preço, limites de minutos/mensagens/dados e tarifas adicionais |

## 📦 Como Executar

1. Clone o repositório:

```bash
git clone https://github.com/rodriguesbrian/tt4_megaline_project
cd tt4_megaline_project