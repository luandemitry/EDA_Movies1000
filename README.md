  # Desafio de Ciência de Dados: Análise Cinematográfica para PProductions

![Status](https://img.shields.io/badge/status-concluído-green)

> Este projeto foi desenvolvido como parte do Desafio de Cientista de Dados da Indicium Lighthouse.O objetivo é analisar uma base de dados cinematográficos para fornecer insights ao estúdio PProductions sobre qual tipo de filme desenvolver, além de construir um modelo de Machine Learning para prever a nota do IMDb de um filme com base em seus atributos.

### 📂 Estrutura do Projeto
O projeto está organizado da seguinte forma para garantir clareza e reprodutibilidade:
```
projeto_filmes_pproductions/
|
|-- data/
|   |-- raw/            # Contém o dataset original
|
|-- models/             # Contém o modelo preditivo salvo (.pkl) e componentes
|
|-- notebooks/          # Contém o Jupyter Notebook com toda a análise
|
|-- reports/            # Contém os gráficos e visualizações geradas
|
|-- README.md           # Documentação do projeto
|-- requirements.txt    # Lista de dependências para instalação
```

### Tecnologias Utilizadas
* Python 3.9+
* Pandas & NumPy para manipulação de dados
* Matplotlib & Seaborn para visualização de dados
* WordCloud para análise de texto
* Scikit-learn para pré-processamento e modelagem
* Jupyter Notebook como ambiente de análise

### Pré-requisitos e Instalação
Para executar este projeto, siga os passos abaixo.

1.  **Clone o repositório:**
    ```bash
    git clone [https://github.com/luandemitry/EDA_Movies1000.git](https://github.com/luandemitry/EDA_Movies1000.git)
    ```

2.  **Crie e ative um ambiente virtual:**
    ```bash
    # Cria o ambiente virtual
    python -m venv .venv

    # Ativa o ambiente (Windows)
    .\.venv\Scripts\activate

    # Ativa o ambiente (macOS/Linux)
    source .venv/bin/activate
    ```

3.  **Instale as dependências:**
    O arquivo `requirements.txt` contém todos os pacotes necessários. Use o pip para instalá-los:
    pip install -r requirements.txt

### Como Executar
Toda a análise, desde a limpeza dos dados até a modelagem, está contida no Jupyter Notebook localizado em `notebooks/eda_inicial.ipynb`.

1.  Inicie o Jupyter Lab ou Jupyter Notebook no seu terminal:
    ```bash
    jupyter lab
    ```
2.  Navegue até a pasta `notebooks/` e abra o arquivo `eda_inicial.ipynb`.
3.  Execute as células do notebook sequencialmente para replicar a análise e os resultados.

### Resumo dos Resultados

A análise exploratória e o modelo preditivo geraram os seguintes insights para a PProductions:

* **Recomendação de Filme:** Para um público geral, um filme do gênero **Drama** com alta avaliação e grande número de votos, como "The Shawshank Redemption", é a recomendação mais segura e aclamada.
* **Fatores de Alto Faturamento:** Os principais fatores relacionados a uma alta bilheteria são:
    * **Gênero:** Filmes de **Ação, Aventura e Animação** possuem as maiores medianas de faturamento.
    * **Engajamento do Público:** Existe uma forte correlação positiva entre o número de votos (`No_of_Votes`) e o faturamento (`Gross`).
* **Modelo Preditivo:** Foi desenvolvido um modelo `RandomForestRegressor` para prever a nota do IMDb. A performance foi avaliada com a métrica **RMSE (Raiz do Erro Quadrático Médio)**, que indica o erro médio do modelo em "pontos de nota".

###  Autor

**Luan Demitry**

* **LinkedIn:** `https://linkedin.com/in/luandemitry`
* **GitHub:** `https://github.com/luandemitry`
