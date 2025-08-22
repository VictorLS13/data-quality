# 🚦 Validação e Qualidade de Dados em Python

Este projeto demonstra como aplicar **verificações de qualidade de dados** em um dataset utilizando **Python**.  
São avaliados três pilares principais da qualidade de dados: **completude, unicidade e validade**, além da geração de **gráficos** para facilitar a interpretação.

---

## 📂 Estrutura do Projeto
- **ValidadorAuxiliar**: Funções de validação específicas (CPF e Email).
- **ValidadorQualidade**: Classe principal que avalia os dados quanto a:
  - **Completude** (valores nulos).
  - **Unicidade** (valores duplicados).
  - **Validade** (CPFs e emails válidos/ inválidos).
- **Visualização**: Gráficos com `matplotlib` para representar os relatórios.

---

## 🛠️ Principais Conceitos Utilizados

### 🔹 Completude
- Mede a **presença de valores nulos** em cada coluna.
- Retorna a contagem e o percentual de campos ausentes.
- Exemplo de visualização: gráfico de barras mostrando **nulos por coluna**.

---

### 🔹 Unicidade
- Verifica a **existência de valores duplicados** em colunas de interesse (ex.: `cpf`).
- Ignora valores nulos na análise.
- Exemplo de visualização: gráfico de barras com **Duplicados x Não Duplicados**.

---

### 🔹 Validade
- Confere se os dados respeitam **padrões formais**:
  - **CPF**: 11 dígitos, não sequencial, e com dígitos verificadores corretos.
  - **Email**: formato válido com `usuario@dominio.com`.
- Retorna a quantidade e percentual de registros válidos e inválidos.
- Exemplo de visualização: gráfico de barras para **CPFs válidos/inválidos** e **Emails válidos/inválidos**.

---

## 📊 Exemplos de Gráficos
- **Completude:** valores nulos por coluna.  
- **Unicidade:** comparação de registros duplicados e não duplicados.  
- **Validade:** CPFs e Emails válidos x inválidos.  

---

## 🛠️ Tecnologias Utilizadas:
Python
Pandas
NumPy
Matplotlib
