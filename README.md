# SENAI/PE – CÓD. 164 PESQUISADOR INDUSTRIAL II (IA Industrial)

Este projeto é parte integrante do Estudo de Caso e contém:

- Código fonte (jupyter notebooks)
- README técnico
- Notebook (ou conjunto de figuras) com a EDA e principais visualizações dos resultados
- Arquivo requirements.txt ou equivalente com as dependências do projeto
- Instruções claras no README para reprodução dos resultados

## Sobre o Projeto

Este repositório contém o código-fonte e os dados utilizados no Estudo de Caso para a vaga **SENAI/PE – CÓD. 164 PESQUISADOR INDUSTRIAL II (IA Industrial)** que consiste em uma prova de conceito de software para um sistema de monitoramento inteligente de ativos rotativos (motores elétricos) em ambiente industrial.

Maiores informações podem ser obtiidas nos documentos de instruções que constam neste repositório na pasta docs.

Este projeto está divivido em dois módulos:

**Módulo 1: EDA e Classificação de Condição do Motor**
**Objetivo:** Demonstrar fundamentos de análise exploratória de dados industriais, engenharia de
features em sinais vibro-acústicos e classificação multiclasse de falhas.

**Observação**: FFT, Feature Engineering, Features no tempo, e Features na frequência, e modelos de classifcação, bem como as análises de resultados foram realizadas com o uso de IA Generativa (Vide Jupyter Notebook).

**Módulo 2: Softsensor de Temperatura (Opcional, bônus)**
**Objetivo:** Demonstrar capacidade de construir softsensors industriais, modelos que inferem o
valor de uma variável difícil, lenta ou cara de medir a partir de outras variáveis disponíveis.

**Observação**: Segue apenas a explicação com o uso de IA Generativa: 

Descrição do Módulo 2 (caso fosse implementado)
Caso o Módulo 2 fosse desenvolvido, ele incluiria a criação de um softsensor de temperatura utilizando técnicas de regressão e modelos supervisionados. O processo envolveria seleção das melhores features, testes com diferentes algoritmos (como Random Forest Regressor, Gradient Boosting ou Redes Neurais), além de tuning de hiperparâmetros para otimização. As métricas utilizadas incluiriam MAE, RMSE e R², garantindo avaliação completa da capacidade preditiva do modelo. O objetivo seria demonstrar como modelos de IA podem estimar variáveis críticas em sistemas industriais, mesmo sem medições diretas.


## Base de Dados
- **Fonte:** Fornecido pelo SENAI-PE para realização do estudo de caso: O dataset é um subset curado do University of Ottawa Electric Motor Dataset — Vibration and
Acoustic Faults under Constant and Variable Speed Conditions (UOEMD-VAFCVS).
- **Download:** [Electric Motor Dataset](https://drive.google.com/file/d/1i1PNKLjWYL6_WzB2rcztGHI_mt4uy-zZ/view?usp=drivesdk)

## Bibliotecas Utilizadas
- `pandas`, `numpy` - Manipulação de dados
- `matplotlib` - Visualização
- `scikit-learn` - Regressão Logística
- `scipy` - Testes estatísticos

## Estrutura do Repositório
```bash
senai-pe-164-pesqindII/
├── data/
│   └── *.csv files
├── images/
│   └── *.png files models and EDA                
├── notebooks/
│   └── *.ipynb files
├── .gitignore
├── README.md
└── requirements.txt
```

## Reprodutibilidade

Este repositório contém todos os elementos necessários para reproduzir os experimentos:

1. **Dados**: Arquivo CSV processado na pasta `data/`
2. **Código**: Jupyter Notebook em `notebooks/`
3. **Dependências**: `requirements.txt`

### Pré-requisitos

- Python 3.13
- VSCode com extensão Jupyter instalada.

### Executando no VSCode
   - Verifique se o Python, Git, e o VSCode estão instalados antes de executar os passos abaixo.

1. Clone o repositório:
   ```bash
   git clone git clone https://github.com/Lima-PPGEP/senai-pe-164-pesqindII
   cd senai-pe-164-pesqindII
   ```

2. Crie e ative o ambiente virtual:

   Windows
   ```bash
   py -3.13 -m venv venv
   venv\Scripts\activate     # Windows
   ```

   Linux
   ```bash
   python3.13 -m venv venv
   source venv/bin/activate
   ```

3. Instale as dependências:
   ```bash
   pip install -r requirements.txt
    ```

4. Em seguida selecione o interpretador no VSCode:
   - Ctrl+Shift+P → Python: Select Interpreter
   - Escolha o caminho onde o ambiente virtual: .\venv\Scripts\python.exe Ex.: SBPO2026-fl-algorithm\venv\Scripts\python.exe

5. Abra o notebook no VSCode:
   - Verifique se o Jupyter Notebook está utilizando o mesmo ambiente virtual (venv) para execução.
   - Faça isso clicando no canto superior direito do Jupyter Notebook deve estar escrito Python (descrição do ambiente virtual)

## Autor do projeto. 
Carlos Lima 
- [GitHub](https://github.com/Lima-PPGEP)
- [LinkedIn](https://www.linkedin.com/in/carlos-lima/)

## Licença
Este projeto está licenciado sob os termos da [Creative Commons Attribution 4.0 (CC-BY 4.0)](LICENSE.md)

## Referências

[Como estrturuar um README.md](https://www.alura.com.br/artigos/escrever-bom-readme)




