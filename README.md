# ⚙️ Power Query M - Funções e Rotinas Dinâmicas

Este repositório centraliza uma biblioteca de funções, métodos e rotinas desenvolvidas em **Linguagem M**, focadas em automação de ETL, otimização de performance e resiliência de dados no Power BI e Excel.

## 🚀 Objetivo
Diferente de fluxos de ETL rígidos, as rotinas aqui presentes foram projetadas para serem **dinâmicas e autoadaptáveis**, minimizando a necessidade de manutenção manual diante de alterações estruturais nas fontes de dados (*Schema Drift*).

---

## 📂 Estrutura do Repositório

O repositório está organizado em subpastas para facilitar a localização e implementação das rotinas:

### 🔹 [Rotina]
Contém scripts completos de processos de ETL ponta a ponta. 
* **Destaque:** Implementações de expansão dinâmica de colunas e algoritmos de tipagem automática que analisam a amostra dos dados para definir o tipo de campo em tempo de execução.

### 🔹 [Funções]
Biblioteca de funções personalizadas (UDFs) para resolver desafios específicos:
* Tratamento de calendários dinâmicos.
* Funções para limpeza de caracteres especiais e padronização de strings.
* Lógicas de cálculos complexos reaproveitáveis em múltiplos modelos.

### 🔹 [Exemplos]
Arquivos ou trechos de código que demonstram a aplicação prática das funções em cenários reais de Business Intelligence.

---

## 🛠️ Diferenciais Técnicos
* **Autoadaptação:** Uso intensivo de `List.Transform`, `List.Combine` e `Table.ColumnNames` para evitar nomes de colunas fixos (*hardcoded*).
* **Robustez:** Implementação de lógicas com `MissingField.Ignore` para garantir que a atualização não seja interrompida por campos ausentes.
* **Performance:** Scripts otimizados para reduzir o consumo de memória e o tempo de processamento durante o *refresh* dos dados.

## 🔗 Como utilizar
Basta copiar o código `.m` desejado, abrir o **Editor Avançado** no Power Query e adaptar as variáveis de entrada (como caminhos de arquivos ou nomes de tabelas).

---
**Desenvolvido por [Tiago Almeida Goulart](https://www.linkedin.com/in/tiago-agoulart)** Analista de People Analytics Sênior | Especialista em Automação e Engenharia de Dados
