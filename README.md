# Projeto_Novas_Tech

## Sobre o projeto

Este projeto tem como objetivo realizar uma análise exploratória de dados imobiliários e preparar a base para aplicações de Machine Learning. O conjunto de dados utilizado contém informações sobre imóveis residenciais, como área, qualidade geral, ano de construção, bairro, número de cômodos, garagem e preço de venda.

O problema principal consiste em compreender quais características dos imóveis podem influenciar o valor de venda (`SalePrice`) e organizar os dados para análises estatísticas, visualizações e futuras etapas de modelagem preditiva ou agrupamento.

## Estrutura do projeto

```text
Projeto_Novas_Tech/
├── banco de dados/
│   ├── train.csv
│   ├── test.csv
│   ├── sample_submission.csv
│   ├── data_description.txt
│   ├── train_tratado.csv
│   └── test_tratado.csv
├── imagens/
│   ├── graficoBarras.png
│   ├── histograma.png
│   ├── boxplot.png
│   ├── graficoDispersao.png
│   └── matrixDeCorrelacao.png
├── Preço_imoveis.ipynb
├── README.md
├── LICENSE
├── .gitignore
└── .gitattributes
```

## Tecnologias utilizadas

- Python: linguagem principal do projeto.
- Jupyter Notebook: ambiente utilizado para executar a análise.
- Pandas: leitura, manipulação, limpeza e exportação dos dados.
- NumPy: apoio para operações numéricas e tratamento de dados.
- Matplotlib: criação e salvamento dos gráficos.
- Scikit-learn:
  - `StandardScaler`: padronização de variáveis numéricas.
  - `KMeans`: algoritmo de agrupamento para possíveis análises de clusters.

## Etapas desenvolvidas

O notebook `Preço_imoveis.ipynb` contempla as seguintes etapas:

1. Descrição do problema.
2. Explicação da base de dados.
3. Importação das bibliotecas.
4. Leitura dos arquivos `train.csv` e `test.csv`.
5. Verificação do número de linhas e colunas.
6. Identificação dos tipos de dados.
7. Visualização de amostras da base.
8. Identificação de valores nulos.
9. Verificação e remoção de dados duplicados.
10. Correção de inconsistências em textos.
11. Ajuste de campos relacionados a anos para formato de data.
12. Geração de estatísticas descritivas:
    - média;
    - mediana;
    - mínimo;
    - máximo;
    - desvio padrão.
13. Salvamento dos datasets tratados.
14. Criação e salvamento de visualizações:
    - gráfico de barras;
    - histograma;
    - boxplot;
    - gráfico de dispersão;
    - matriz de correlação.

## Como executar o projeto

### 1. Clonar ou baixar o repositório

Abra o projeto na pasta:

```bash
C:\Projeto_Novas_Tech
```

### 2. Criar um ambiente virtual

No terminal, dentro da pasta do projeto, execute:

```bash
python -m venv .venv
```

### 3. Ativar o ambiente virtual

No Windows PowerShell:

```bash
.venv\Scripts\Activate.ps1
```

No Prompt de Comando:

```bash
.venv\Scripts\activate.bat
```

### 4. Instalar as dependências

```bash
pip install pandas numpy matplotlib scikit-learn notebook
```

### 5. Abrir o Jupyter Notebook

```bash
jupyter notebook
```

Em seguida, abra o arquivo:

```text
Preço_imoveis.ipynb
```

### 6. Executar as células

Execute as células do notebook em ordem, de cima para baixo. O notebook realiza a leitura dos dados, análise exploratória, tratamento básico, geração de estatísticas e criação dos gráficos.

## Arquivos gerados

Após a execução do notebook, são gerados os seguintes arquivos:

```text
banco de dados/train_tratado.csv
banco de dados/test_tratado.csv
imagens/graficoBarras.png
imagens/histograma.png
imagens/boxplot.png
imagens/graficoDispersao.png
imagens/matrixDeCorrelacao.png
```

## Observações

O projeto ainda está em fase de análise exploratória. As bibliotecas `StandardScaler` e `KMeans`, do Scikit-learn, podem ser utilizadas em uma próxima etapa para padronizar variáveis numéricas e agrupar imóveis com características semelhantes.

## Licença

Este projeto está sob a licença MIT. Consulte o arquivo `LICENSE` para mais detalhes.
