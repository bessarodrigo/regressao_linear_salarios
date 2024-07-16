# Análise de Fatores Influentes no Salário

Este repositório contém uma análise detalhada dos fatores que influenciam os salários dos colaboradores de uma empresa. Técnicas de regressão linear múltipla foram utilizadas para identificar e quantificar a influência da educação superior, tempo na empresa, experiência em outras empresas e conhecimento de inglês sobre o salário dos colaboradores.

## Estrutura do Repositório

- **base_salarios.xlsx**: Arquivo de dados utilizado para a análise.
- **produtos_naturais.ipynb**: Script Python contendo todo o processo de análise, desde a importação e tratamento dos dados até a construção e interpretação do modelo de regressão.
- **README.md**: Este arquivo, contendo a descrição do problema de negócio e instruções sobre como utilizar o repositório.

## Instalação e Execução

### Requisitos

- Python 3.6 ou superior
- Bibliotecas Python: numpy, pandas, matplotlib, seaborn, statsmodels, scipy

### Passos para Execução

1. Clone este repositório:

    ```bash
    git clone https://github.com/bessarodrigo/regressao_linear_salarios.git
    cd regressao_linear_salarios
    ```

2. Instale as bibliotecas necessárias:

    ```bash
    pip install numpy pandas matplotlib seaborn statsmodels scipy
    ```

3. Execute o script de análise:

    ```bash
    python analysis_script.py
    ```

## Descrição do Script

### Importação e Tratamento dos Dados

- Os dados são carregados a partir de um arquivo Excel (base_salarios.xlsx).
- Colunas desnecessárias são removidas, e as colunas restantes são renomeadas para facilitar a análise.
- Estatísticas descritivas e visualizações iniciais são criadas para entender melhor a distribuição dos dados.

### Análise Exploratória

- Histogramas e box plots são utilizados para explorar a distribuição dos salários.
- Estatísticas descritivas são geradas para variáveis como anos de educação superior, tempo na empresa e tempo em outras empresas.
- Um gráfico de barras é criado para mostrar a distribuição de pessoas que falam ou não falam inglês.

### Análise Bidimensional

- Gráficos de dispersão com linhas de tendência são criados para explorar a relação entre salário e outras variáveis (anos de educação superior, tempo na empresa e tempo em outras empresas).
- Coeficientes de correlação de Pearson são calculados e exibidos nos gráficos.

### Regressão Linear Múltipla

- Variáveis dummy são criadas para a variável categórica `Ingles`.
- Um modelo de regressão linear múltipla é ajustado utilizando as variáveis `Anos_Educ_Superior`, `Tempo_Empresa`, `Tempo_Outras_Empresas` e `Ingles_Sim`.
- Com base nos resultados, variáveis não significativas são removidas, e o modelo é ajustado novamente.

### Interpretação do Modelo

- A equação do modelo é apresentada, e os coeficientes são interpretados para fornecer insights práticos sobre como cada fator influencia o salário dos colaboradores.

## Contribuição

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues e pull requests.

## Contato
LinkedIn: https://www.linkedin.com/in/rodrigo-bessa/
