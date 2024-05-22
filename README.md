# Projeto Machine Learning 2: Ada Santander Coders 2023.2
_Projeto feito para conclusão do módulo de Machine Learning 2, do Santander Coders 2023.2 | Ada_
**Professor:** Jorge Chamby-Diaz

## Como executar este projeto
O projeto foi desenvolvido utilizando o ambiente base do [Anaconda](https://www.anaconda.com/products/navigator). Sendo necessário apenas um ambiente como o `conda` ou [`Miniconda`](https://docs.anaconda.com/free/miniconda/).

### Executando com VENV
Alternativamente, é possível utilizar um ambiente virtual com `venv`. As bibliotecas necessárias estão no arquivo `requirements.txt`. Basta seguir o seguinte passo a passo:

1. No `powershell`, `bash` ou `cmd`, navegue até o diretório raiz do projeto.

2. Crie um ambiente virtual com o comando
```powershell
python -m venv .venv
```

3. Ative o ambiente virtual. O comando pode diferir a depender do seu sistema operacional.
O exemplo abaixo é para ativação via `CMD`
```cmd
.venv\Scripts\activate.bat
```

4. Instale as dependências com `pip`
```cmd
pip install -r .\requirements.txt
```

## Base de dados
Foram utilizadas algumas das base de dados disponibilizadas em [Covid 19 BR](https://github.com/wcota/covid19br/), lida diretamente do `github` do projeto. Utilizando `pandas`, pode ser feito da seguinte forma:

```python
pd.read_csv('https://raw.githubusercontent.com/wcota/covid19br/master/cases-brazil-states.csv')
```

## Notebook
O notebook que contem as atividades necessárias ao projeto encontra-se na raiz deste diretório, e pode ser acessado aqui: [Projeto](project_ml2.ipynb)

### Gráficos Pesados
Alguns gráficos mais pesados, como os do `sns.pairplot()` ou os produzidos pelo `plotly` podem ser mais lentos para reproduzir. Por isso, cópias desses gráficos estão disponíveis no diretório [`plots`](./plots/).

## TO-DO:
- [X] Apresentação da Análise:
    - [X] Storytelling;
    - [X] Insights (Padrões que descrevam os elementos da base);
    - [X] Descrição do problema;
    - [ ] Proposta de solução;
- [ ] Entregáveis:
    - [X] Relatório com análise exploratória de dados;
        - [X] Descrição das variáveis (dados faltantes, tipos de dados, informações relacionadas e fontes);
        - [X] Limpeza da base;
    - [X] Análise Univariada e Multivariada:
        - [X] Medidas estatísticas;
        - [X] Comparações;
        - [ ] Tendências de crescimento ou queda;
    - [X] Gráficos;
    - [ ] Segmentação dos dados (agrupamentos em relação a variáveis de interesse);
    - [ ] Análise Preditiva (utilzação de modelos para predizer variáveis de interesse dos problemas levantados)

