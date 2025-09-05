# Page View Time Series Visualizer

Solução completa para o projeto "Page View Time Series Visualizer" do freeCodeCamp, parte da certificação Data Analysis with Python.

## Sobre o Projeto

Visualização de dados de séries temporais do fórum freeCodeCamp.org mostrando visualizações de página diárias de maio 2016 até dezembro 2019. O projeto gera três tipos de gráficos para análise de tendências e padrões sazonais.

## Implementações

### 1. Script Python (`time_series_visualizer.py`)
- Código limpo para submissão no freeCodeCamp
- Três funções principais: `draw_line_plot()`, `draw_bar_plot()`, `draw_box_plot()`
- Gera automaticamente as imagens dos gráficos

### 2. Jupyter Notebook (`page_view_visualizer.ipynb`)
- Análise exploratória completa
- 21 células organizadas com explicações detalhadas
- Estatísticas descritivas e insights dos dados
- Ideal para aprendizado

## Visualizações Geradas

1. **Line Plot**: Gráfico de linha com visualizações diárias ao longo do tempo
2. **Bar Plot**: Médias mensais agrupadas por ano com legendas coloridas
3. **Box Plots**: Tendência anual e sazonalidade mensal em gráficos lado a lado

## Instalação

```bash
pip install pandas matplotlib seaborn numpy jupyter
```

## Como Usar

### Script Python
```python
python time_series_visualizer.py
```

### Jupyter Notebook
```bash
jupyter notebook
# Abrir page_view_visualizer.ipynb
```

## Dataset

Necessário o arquivo `fcc-forum-pageviews.csv` com colunas:
- `date`: Data no formato YYYY-MM-DD
- `value`: Número de visualizações

## Funcionalidades

- Limpeza automática de dados removendo outliers (percentis 2.5% e 97.5%)
- Parsing correto de datas com pandas
- Formatação profissional dos gráficos
- Salvamento automático das imagens em PNG
- Compatível com testes automatizados do freeCodeCamp

## Arquivos de Saída

- `line_plot.png`
- `bar_plot.png` 
- `box_plot.png`
