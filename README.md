# Análise ESG de Startups com Machine Learning

Este projeto aplica técnicas de aprendizado de máquina não supervisionado para análise de dados ESG (Environmental, Social, and Governance) de startups, utilizando algoritmos de clustering e redução de dimensionalidade.

## 📊 Sobre o Projeto

O projeto investiga padrões em dados ESG de startups utilizando diferentes abordagens de análise e visualização. Os experimentos incluem:

- **K-Means Clustering**: Agrupamento de startups com base em métricas ESG
- **Self-Organizing Maps (SOM)**: Clustering topológico com MiniSOM
- **PCA & t-SNE**: Redução de dimensionalidade para visualização
- **Visualizações interativas**: Análise exploratória com Plotly e Matplotlib

## 🗂️ Estrutura do Projeto

```
.
├── data/
│   └── StartUpsESG_0602.csv          # Dataset com dados ESG de startups
├── notebooks/
│   ├── experimento_1.ipynb           # Análise com K-Means, PCA e t-SNE
│   ├── vhdc.ipynb                    # Experimento de clustering hierárquico
│   ├── minisom-experiment.ipynb      # Implementação com Self-Organizing Maps
│   └── Visualizacao.ipynb            # Visualizações e análises exploratórias
├── requirements.txt                   # Dependências do projeto
└── README.md
```

## 📈 Datasets

O projeto utiliza o dataset `StartUpsESG_0602.csv` contendo:

- **StartUp**: Nome da startup
- **Country**: País de origem
- **ESG**: Pontuação ESG geral
- **E**: Pontuação Ambiental (Environmental)
- **S**: Pontuação Social (Social)
- **G**: Pontuação de Governança (Governance)
- **Raised**: Capital levantado

## 🧪 Notebooks

### 1. experimento_1.ipynb
Análise principal com:
- Pré-processamento e normalização dos dados (StandardScaler)
- K-Means clustering para identificação de grupos
- PCA para redução de dimensionalidade
- t-SNE para visualização em 2D/3D
- Visualizações interativas com Plotly

### 2. minisom-experiment.ipynb
Implementação de Self-Organizing Maps:
- Normalização com MinMaxScaler
- Treinamento de SOM (2x2 grid)
- Visualização de mapas de distância
- Análise topológica dos clusters

### 3. vhdc.ipynb
Experimento com clustering hierárquico:
- Feature scaling avançado
- Análise de componentes principais
- Clustering baseado em múltiplas métricas

### 4. Visualizacao.ipynb
Análise exploratória e visualizações:
- Estatísticas descritivas
- Distribuições de features
- Correlações entre variáveis ESG
- Gráficos comparativos por país

## 🚀 Como Usar

### Pré-requisitos

- Python 3.8+
- Jupyter Notebook ou JupyterLab

### Instalação

1. Clone o repositório:
```bash
git clone https://github.com/saimontavares/codespaces-jupyter.git
cd codespaces-jupyter
```

2. Instale as dependências:
```bash
pip install -r requirements.txt
```

3. Instale o MiniSOM (necessário para minisom-experiment.ipynb):
```bash
pip install minisom
```

### Executando os Notebooks

1. Inicie o Jupyter:
```bash
jupyter notebook
```

2. Navegue até a pasta `notebooks/` e abra o notebook desejado

3. Execute as células sequencialmente (Shift + Enter)

## 📦 Dependências Principais

```
pandas==1.5.3          # Manipulação de dados
numpy==1.24.2          # Computação numérica
matplotlib==3.7.0      # Visualizações básicas
torch==2.4.0           # Deep Learning (PyTorch)
scikit-learn           # Machine Learning (implícito)
plotly                 # Visualizações interativas
minisom                # Self-Organizing Maps
```

## 🔬 Metodologia

1. **Pré-processamento**:
   - Tratamento de valores ausentes
   - Normalização com StandardScaler/MinMaxScaler
   - Separação de features categóricas e numéricas

2. **Feature Engineering**:
   - Scaling das métricas ESG (E, S, G)
   - Normalização do capital levantado (Raised)

3. **Clustering**:
   - K-Means para identificação de grupos
   - SOM para análise topológica
   - Validação com métricas de silhueta

4. **Visualização**:
   - Redução para 2D/3D com PCA e t-SNE
   - Gráficos interativos com Plotly
   - Heatmaps e mapas de distância

## 📊 Resultados

Os notebooks demonstram:
- Agrupamento natural de startups por perfil ESG
- Correlações entre métricas ambientais, sociais e de governança
- Padrões geográficos na adoção de práticas ESG
- Relação entre pontuação ESG e capital levantado

## 🤝 Contribuindo

Contribuições são bem-vindas! Sinta-se à vontade para:
- Reportar bugs
- Sugerir novas análises
- Adicionar novos experimentos
- Melhorar visualizações

## 📝 Licença

Este projeto está sob a licença especificada no arquivo [LICENSE](LICENSE).

## 👤 Autor

**Saimon Tavares**
- GitHub: [@saimontavares](https://github.com/saimontavares)

## 🔗 Links Úteis

- [Documentação Scikit-learn](https://scikit-learn.org/)
- [MiniSOM GitHub](https://github.com/JustGlowing/minisom)
- [Plotly Python](https://plotly.com/python/)
- [ESG Metrics Guide](https://www.msci.com/esg-101-what-is-esg)

---

⭐ Se este projeto foi útil, considere dar uma estrela no repositório!
