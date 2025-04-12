## Sobre o Projeto
Este projeto utiliza regressão linear para analisar os fatores que influenciam o salário de profissionais. A análise considera variáveis como educação, tempo de empresa e fluência em inglês, e é complementada por testes estatísticos que validam os pressupostos do modelo.

## Estrutura do Repositório

- ├── data/ # Arquivos de dados originais
- ├── notebooks/ # Análises exploratórias e modelagem
- ├── src/ # Funções e módulos reutilizáveis
- ├── README.md
- └── requirements.txt

## Etapas do Projeto
#### 1. 📦 Tratamento dos Dados
- Remoção de colunas desnecessárias (como o número de identificação do funcionário)
- Mudança nos nomes das colunas para deixar as variáveis mais intuitivas
- Conversão de variáveis categóricas em dummies
- Criação de colunas auxiliares (ex: intercepto)

### 2. 🔍 Análise Univariada
- Estatísticas descritivas para cada variável
- Histogramas e boxplots para identificar outliers e avaliar o comportamento da amostra

### 3. 🔗 Análise Bivariada
- Comparações entre a variável salário e variáveis explicativas
- Correlações e gráficos de dispersão

### 4. 📉 Modelo de Regressão
- Avaliação dos coeficientes e significância estatística
- Eliminação da variável `Tempo_Outras_Empresas` com base no p-valor (acima de 5%)

### 5. 🧪 Diagnóstico do Modelo
#### Homocedasticidade  
- Gráfico dos resíduos padronizados  
- Teste de White (p-valor > 5% = não rejeita H₀ → homocedasticidade)
#### Normalidade dos Resíduos  
- Histograma dos resíduos  
- Teste de Shapiro-Wilk (p-valor > 5% = resíduos seguem distribuição normal)

## 📊 Conclusões
- As variáveis `Anos_Educ_Superior`, `Tempo_Empresa` e `Ingles_Sim` influenciam de forma significativa o salário
- O modelo passou no teste de homocedasticidade
- O teste de normalidade dos resíduos indicou leve desvio da normalidade

## Contato
LinkedIn: https://www.linkedin.com/in/rodrigo-bessa/
