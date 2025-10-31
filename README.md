# 📈 Análise de Performance de Estudantes: Qual Fator Prediz o Sucesso?

## ✨ Visão Geral do Projeto

Este projeto de Análise de Dados tem como foco principal **quantificar o impacto de hábitos de estudo e de vida (horas estudadas, horas de sono e frequência) na nota final de estudantes**.

O objetivo foi construir um pipeline completo, desde a estruturação de um banco de dados otimizado até a visualização de insights em um dashboard interativo.

## 🔑 Insight Chave (O Ponto Focal da Análise)

A análise estatística demonstrou que o **Tempo de Estudo é o fator mais forte e confiável** para prever o desempenho final:

| Relação | Coeficiente de Correlação (DAX) | Interpretação |
| :--- | :--- | :--- |
| **Horas Estudadas vs. Nota Final** | **+0,78** | **Correlação Positiva Forte** (Maior indicador de sucesso) |
| Horas de Sono vs. Nota Final | Baixa/Fraca | Hábito com impacto marginal na nota. |
| Frequência vs. Nota Final | Baixa/Fraca | Hábito com impacto marginal na nota. |

## 🛠️ Stack Tecnológico e Metodologia

Este projeto demonstra proficiência em todas as etapas da análise de dados:

### 1. Modelagem e Otimização de Dados (SQL)

* **Criação de Schema:** Definição da tabela `estudantes` com tipos de dados `DECIMAL` para cálculos precisos.
* **Otimização de Performance:** Criação de **Índices** (Ex: `idx_hours_studied`, `idx_exam_score`) para acelerar drasticamente as consultas de agregação (`GROUP BY` e `CASE WHEN`).
* **Lógica de Negócio:** Uso de comandos `CASE WHEN` para criar **faixas de rendimento** (`Alto Estudo`, `Baixo Estudo`) e realizar análises de impacto dentro do banco de dados.

### 2. Análise e Visualização (Power BI & DAX)

* **Modelagem DAX:** Implementação de medidas complexas (fórmulas universais de Covariância/Desvio Padrão) para calcular o **Coeficiente de Correlação (+0,78)**.
* **Dashboard Interativo:** Construção de um layout otimizado (filtros horizontais no topo) que permite ao usuário filtrar o dataset e visualizar:
    * Distribuição de alunos por faixas de notas.
    * Média de notas em cada grupo de hábitos.
* **Design:** Uso de paleta de cores escura/profissional e destaque visual para o KPI principal.

### 3. Dashboard Online

(https://app.powerbi.com/view?r=eyJrIjoiZDA3MzExNGMtYmY4NC00MmMxLThlZGUtNTVmZmFiNzgzZmFjIiwidCI6ImMwMTRhZWVjLTFiZTAtNGFkMC04MDdhLWRiMGQ3YzJhMTAzZCJ9)

---
*Este projeto demonstra a capacidade de transformar requisitos de negócio em modelos de dados robustos e insights acionáveis.*
