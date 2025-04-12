# 📈 Salary Prediction with Linear Regression

## 📝 Sobre o Projeto  
Este projeto utiliza **regressão linear** para analisar os fatores que influenciam o salário de profissionais. A análise considera variáveis como **educação**, **tempo de empresa** e **fluência em inglês**, e é complementada por testes estatísticos que validam os pressupostos do modelo.

---

## 📁 Estrutura do Repositório

- ├── data/ # Arquivos de dados originais
- ├── notebooks/ # Análises exploratórias e modelagem
- ├── src/ # Funções e módulos reutilizáveis
- ├── README.md
- └── requirements.txt

## 🔄 Etapas do Projeto

### 1. 📦 Tratamento dos Dados  
- Remoção de colunas desnecessárias (ex: número de identificação do funcionário)  
- Renomeação de colunas para nomes mais intuitivos  
- Conversão de variáveis categóricas em dummies  
- Criação de colunas auxiliares (ex: intercepto)  

---

### 2. 🔍 Análise Univariada  
- Estatísticas descritivas para cada variável  
- Histogramas e boxplots para identificar outliers e avaliar a distribuição  

---

### 3. 🔗 Análise Bivariada  
- Comparações entre a variável `Salario` e as variáveis explicativas  
- Cálculo de correlações e gráficos de dispersão  

---

### 4. 📉 Modelo de Regressão  
- Avaliação dos coeficientes e significância estatística  
- Eliminação da variável `Tempo_Outras_Empresas` com base no p-valor (> 0.05)  

---

### 5. 🧪 Diagnóstico do Modelo

#### ✅ Homocedasticidade  
- Gráfico dos resíduos padronizados  
- Teste de White (p-valor > 0.05 → **não rejeita H₀** → homocedasticidade)

#### 📊 Normalidade dos Resíduos  
- Histograma dos resíduos  
- Teste de Shapiro-Wilk (p-valor < 0.05 → **rejeita H₀** → evidência de não-normalidade)

---

## 📊 Conclusões  
- As variáveis `Anos_Educ_Superior`, `Tempo_Empresa` e `Ingles_Sim` influenciam significativamente o salário  
- O modelo passou no teste de homocedasticidade  
- O teste de normalidade dos resíduos indicou **leve desvio da normalidade**  

---

## 📬 Contato  
🔗 [LinkedIn - Rodrigo Bessa](https://www.linkedin.com/in/rodrigo-bessa/)
