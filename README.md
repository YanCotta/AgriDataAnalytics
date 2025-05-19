# FIAP - Faculdade de Informática e Administração Paulista

<p align="center">
<a href= "https://www.fiap.com.br/"><img src="./assets/logo-fiap.png" alt="FIAP - Faculdade de Informática e Admnistração Paulista" border="0" width=40% height=40%></a>
</p>

<br>

# Nome do projeto

## Nome do grupo

## 👨‍🎓 Integrantes

- [Yan Cotta](https://www.linkedin.com/in/yan-cotta/)

## 👩‍🏫 Professores

### Tutor(a)

- Lucas Gomes Moreira

### Coordenador(a)

- André Godoi Chiovato

## 📜 Descrição

O projeto AgriDataAnalytics é uma análise avançada de dados agrícolas para otimizar a seleção de culturas com base em condições de solo (nitrogênio, fósforo, potássio, pH) e clima (temperatura, umidade, precipitação). Desenvolvido como parte de um curso de IA/ML, o projeto utiliza o dataset Atividade_Cap_14_produtos_agricolas.csv para realizar Análise Exploratória de Dados (AED), análise descritiva, definição de perfis ideais de solo/clima e construção de modelos preditivos. O objetivo é fornecer insights acionáveis para agricultores, identificando as condições ideais para culturas como arroz, milho e café, e prever a cultura mais adequada para um dado conjunto de condições.

O notebook main.ipynb implementa uma pipeline completa, incluindo:

- **AED**: Exploração de distribuições e correlações, com histogramas e matriz de correlação.
- **Análise Descritiva**: Visualizações como scatter plots (temperatura vs. umidade) e box plots (pH por cultura), destacando preferências específicas de cada cultura.
- **Modelagem Preditiva**: Cinco modelos (Árvore de Decisão, Floresta Aleatória, SVM, KNN, Rede Neural) foram treinados, com a Floresta Aleatória alcançando a melhor acurácia (>95%). Validação cruzada e análise de importância de características reforçam a robustez dos resultados.
- **Conclusões**: Temperatura e umidade são os principais preditores, enquanto culturas como arroz requerem alta precipitação e nitrogênio. Recomendações práticas incluem condições ideais para culturas específicas.

**Estado Atual**: O projeto está em fase de finalização, com o notebook aprimorado, visualizações geradas (matrizes de confusão, histogramas, scatter plots, etc.) e análises estatísticas iniciais (ex.: ANOVA para temperatura). Limitações incluem a ausência de dados temporais e validação limitada, mas o trabalho é robusto e pronto para entrega acadêmica e inclusão em portfólios.

**Principais Descobertas**:

- Culturas apresentam requisitos distintos, com temperatura e umidade como fatores críticos.
- Floresta Aleatória é o modelo mais eficaz, com alta acurácia e baixa confusão entre culturas.
- Perfis ideais identificados: arroz (N>80, precipitação>200 mm), milho (pH 6.0-7.0), café (K>40, umidade 60-80%).

**Futuro**: Incorporar dados sazonais, explorar engenharia de características (ex.: índices N/P) e implementar mais validação cruzada.

## 📁 Estrutura de pastas

```
AgriDataAnalytics/
├── assets/               # Recursos visuais (imagens, logos)
│   └── logo-fiap.png     # Logo da FIAP
├── data/                 # Dados brutos e processados
│   └── Atividade_Cap_14_produtos_agricolas.csv  # Dataset principal
├── notebooks/            # Jupyter Notebooks com a análise
│   └── main.ipynb       # Notebook principal com toda a análise
├── README.md             # Documentação do projeto
└── requirements.txt      # Dependências do projeto
```

### Descrição dos Diretórios

- `assets/` - Contém recursos visuais como imagens e logos usados no projeto
- `data/` - Armazena o dataset principal em formato CSV
- `notebooks/` - Contém o notebook Jupyter (`main.ipynb`) com toda a análise de dados

### Arquivos na Raiz

- `README.md` - Documentação completa do projeto
- `requirements.txt` - Lista de dependências Python necessárias para executar o projeto

## 🔧 Como executar o código

### Pré-requisitos

- Python 3.9 ou superior
- Bibliotecas listadas em requirements.txt (pandas==2.2.2, numpy==1.26.4, matplotlib==3.9.2, seaborn==0.13.2, scikit-learn==1.5.2, scipy==1.14.1)
- Jupyter Notebook ou JupyterLab
- Windows, macOS ou Linux
- Git para clonar o repositório

### Passo a Passo

1. **Clonar o Repositório**

   ```bash
   git clone https://github.com/seu_usuario/AgriDataAnalytics.git
   cd AgriDataAnalytics
   ```

2. **Instalar Dependências**

   ```bash
   pip install -r requirements.txt
   ```

3. **Executar o Notebook**

   ```bash
   jupyter notebook src/notebooks/main.ipynb
   ```

4. **Verificar Visualizações**

   - As visualizações são salvas em `src/visualizations/`
   - Execute todas as células do notebook para regenerá-las, se necessário

### Notas

- Certifique-se de que o dataset `Atividade_Cap_14_produtos_agricolas.csv` está em `src/data/`
- Para exportar o notebook como PDF

  ```bash
  jupyter nbconvert --to pdf src/notebooks/main.ipynb
  ```

## 🗃 Histórico de lançamentos

### 0.5.0 - 19/05/2025

- Finalização do notebook com AED completa, visualizações descritivas, validação cruzada e análise de importância de características
- Estruturação do repositório e README profissional

### 0.4.0 - 18/05/2025

- Adição de visualizações descritivas (scatter plots, box plots) e relatório em markdown
- Implementação de recomendações práticas por cultura

### 0.3.0 - 17/05/2025

- Treinamento e avaliação de cinco modelos preditivos, com matrizes de confusão
- Análise inicial de temperatura via ANOVA

### 0.2.0 - 16/05/2025

- Exploração inicial dos dados (AED) com histogramas e matriz de correlação
- Pré-processamento com LabelEncoder e StandardScaler

### 0.1.0 - 15/05/2025

- Criação do repositório e importação do dataset
- Estrutura inicial do notebook main.ipynb

## 📋 Licença

Este projeto está licenciado sob a Licença MIT - veja o arquivo [LICENSE](LICENSE) para detalhes.


