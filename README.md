# Page View Time Series Visualizer

Este repositório contém duas implementações completas do projeto "Page View Time Series Visualizer" do freeCodeCamp, que faz parte da certificação **Data Analysis with Python**.

## Sobre o Projeto

O projeto consiste em visualizar dados de séries temporais do fórum freeCodeCamp.org, mostrando o número de visualizações de página diárias de maio de 2016 até dezembro de 2019. O objetivo é criar três tipos diferentes de visualizações para analisar tendências e padrões sazonais nos dados.

## Objetivos

- Importar e limpar dados de séries temporais
- Remover outliers (2.5% superiores e inferiores)
- Criar visualizações profissionais usando matplotlib e seaborn
- Gerar três tipos de gráficos: linha, barras e box plots

## Estrutura do Projeto

```
page-view-time-series-visualizer/
├── README.md
├── time_series_visualizer.py        # Versão script Python
├── page_view_visualizer.ipynb       # Versão Jupyter Notebook
├── fcc-forum-pageviews.csv         # Dataset (não incluído)
├── requirements.txt                 # Dependências
└── outputs/
    ├── line_plot.png
    ├── bar_plot.png
    └── box_plot.png
```

## Duas Implementações Disponíveis

### 1. Versão Script Python (`time_series_visualizer.py`)

**Características:**
- Código limpo e direto para submissão no freeCodeCamp
- Três funções principais: `draw_line_plot()`, `draw_bar_plot()`, `draw_box_plot()`
- Salva automaticamente as imagens dos gráficos
- Ideal para ambiente de produção

**Como usar:**
```python
import time_series_visualizer as tsv

# Gerar todos os gráficos
line_fig = tsv.draw_line_plot()
bar_fig = tsv.draw_bar_plot()
box_fig = tsv.draw_box_plot()
```

### 2. Versão Jupyter Notebook (`page_view_visualizer.ipynb`)

**Características:**
- Análise exploratória completa dos dados
- Explicações detalhadas de cada etapa
- Visualizações inline para análise imediata
- Estatísticas descritivas e insights
- 21 células organizadas didaticamente
- Ideal para aprendizado e análise

**Conteúdo do Notebook:**
- Importação e configuração das bibliotecas
- Carregamento e limpeza dos dados com estatísticas
- Criação dos três tipos de gráficos
- Análise detalhada dos resultados
- Código final pronto para submissão

## Visualizações Geradas

### 1. Line Plot
- **Arquivo:** `line_plot.png`
- **Descrição:** Gráfico de linha mostrando visualizações diárias ao longo do tempo
- **Período:** Maio 2016 - Dezembro 2019
- **Objetivo:** Identificar tendências gerais e picos de tráfego

### 2. Bar Plot
- **Arquivo:** `bar_plot.png`
- **Descrição:** Gráfico de barras com médias mensais agrupadas por ano
- **Formato:** Barras por ano, cores diferentes para cada mês
- **Objetivo:** Comparar sazonalidade entre diferentes anos

### 3. Box Plots
- **Arquivo:** `box_plot.png`
- **Descrição:** Dois box plots lado a lado
  - **Esquerda:** Tendência por ano (Year-wise Box Plot)
  - **Direita:** Sazonalidade por mês (Month-wise Box Plot)
- **Objetivo:** Analisar distribuições e identificar outliers

## Instalação e Configuração

### Pré-requisitos
- Python 3.7+
- pip (gerenciador de pacotes Python)

### Instalação das Dependências

```bash
# Clonar o repositório (se aplicável)
git clone <repository-url>
cd page-view-time-series-visualizer

# Instalar dependências
pip install -r requirements.txt
```

### Dependências Principais
```
pandas>=1.3.0
matplotlib>=3.4.0
seaborn>=0.11.0
numpy>=1.21.0
jupyter>=1.0.0  # Para a versão notebook
```

## Dataset

O projeto utiliza o arquivo `fcc-forum-pageviews.csv` que deve conter:
- **Coluna `date`:** Data no formato YYYY-MM-DD
- **Coluna `value`:** Número de visualizações de página

**Estrutura esperada:**
```csv
date,value
2016-05-09,19736
2016-05-10,19459
...
```

## Como Usar

### Opção 1: Script Python

1. Certifique-se de ter o arquivo `fcc-forum-pageviews.csv` no diretório
2. Execute o script:

```python
python time_series_visualizer.py
```

3. Os gráficos serão salvos automaticamente como PNG

### Opção 2: Jupyter Notebook

1. Inicie o Jupyter Notebook:
```bash
jupyter notebook
```

2. Abra o arquivo `page_view_visualizer.ipynb`
3. Execute cada célula sequencialmente (Shift + Enter)
4. Analise os resultados e gráficos gerados

## Funcionalidades Implementadas

### Limpeza de Dados
- Parsing correto de datas
- Remoção de outliers (percentis 2.5% e 97.5%)
- Tratamento de dados ausentes
- Validação da estrutura dos dados

### Visualizações
- Line plot com formatação de datas
- Bar plot com legendas e cores apropriadas
- Box plots duplos para tendência e sazonalidade
- Títulos, labels e formatação profissional
- Salvamento automático em alta resolução

### Análise (Versão Notebook)
- Estatísticas descritivas completas
- Identificação de picos e valores extremos
- Análise temporal por ano e mês
- Insights sobre padrões sazonais

## Compatibilidade freeCodeCamp

Ambas as implementações foram testadas e são compatíveis com os testes automatizados do freeCodeCamp. O código da versão script pode ser copiado diretamente para a plataforma.

### Requisitos Atendidos:
- Importação correta dos dados com parsing de datas
- Limpeza dos dados removendo outliers
- Três funções de visualização implementadas
- Títulos e labels corretos conforme especificação
- Salvamento das imagens nos nomes esperados
- Formatação e estilos apropriados

## Contribuição

Contribuições são bem-vindas! Se você encontrar bugs ou tiver sugestões de melhorias:

1. Faça um fork do projeto
2. Crie uma branch para sua feature (`git checkout -b feature/AmazingFeature`)
3. Commit suas mudanças (`git commit -m 'Add some AmazingFeature'`)
4. Push para a branch (`git push origin feature/AmazingFeature`)
5. Abra um Pull Request

## Licença

Este projeto é desenvolvido para fins educacionais como parte da certificação freeCodeCamp Data Analysis with Python.

## Links demasiademtnte úteis (para quem quiser fazer isso também)

- [freeCodeCamp - Data Analysis with Python](https://www.freecodecamp.org/learn/data-analysis-with-python/)
- [Documentação Pandas](https://pandas.pydata.org/docs/)
- [Documentação Matplotlib](https://matplotlib.org/stable/contents.html)
- [Documentação Seaborn](https://seaborn.pydata.org/)

## Autor

Desenvolvido como solução para o projeto freeCodeCamp "Page View Time Series Visualizer".

---

**Nota:** Certifique-se de baixar o dataset `fcc-forum-pageviews.csv` do site oficial do freeCodeCamp antes de executar o código.