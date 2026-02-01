# Análise de Voo: Nashira vs. Simulação RocketPy

Este repositório contém a resolução do *Desafio de Payload* referente ao Processo Seletivo da *EPTA* (Equipe de Propulsão e Tecnologia Aeroespacial) - UFU.

O projeto consiste na análise pós-voo dos dados de telemetria do foguete *Nashira*, comparando-os com uma simulação de referência realizada com a biblioteca *RocketPy*.

## Objetivos
1.  **Processamento de Dados:** Limpeza e tratamento de dados da telemetria.
2.  **Simulação Comparativa:** Utilização do modelo **Calisto** para análise do voo de um foguete.
3.  **Análise de Voo:** Identificação de anomalias (falha de recuperação, perda de dados) através da discrepância entre o modelo ideal e dos dados reais.


## Principais resultados 
* Apogeu Real: ~283 metros (identificado via barômetro, com filtro).
* Problema na queda: Falha no sistema de recuperação (paraquedas), evidenciada pelo perfil de descida, com alta velocidade de impacto.
* Previsão de Pouso: Através da extrapolação dos dados de altitude, estimou-se o final da queda

## Ferramentas
* **Python 3.12.3**
* **RocketPy** (Simulação da Dinâmica de Voo)
* **Pandas & NumPy** (Manipulação dos dados em arquivo .csv e cálculos envolvendo vetores)
* **Matplotlib** (Plotagem de gráficos)
* **Scikit-learn** (Regressão linear)

## 📂 Estrutura do Repositório
* `challenge_rocketpy.ipynb`: Jupyter Notebook que contém todo o código de análise, gráficos e discussões.
* `nashira_flight_data.csv`: Dados de telemetria do voo real.
* `Cesaroni_M1670.eng`: Arquivo de curva de empuxo do motor utilizado na simulação.
* `powerOffDragCurve.csv` e `powerOnDragCurve.csv`: Arquivos do foguete.
* `requirements.txt`: Lista de dependências.

## Execução
1. Clone o repositório:
    ```
    git clone https://github.com/alexburdelis/rocketpy-and-telemetry-analysis-Public.git
    ```
2. Instale dependências:
    ```
    pip install -r requirements.txt
    ```
3. Abra o notebook:
    ```
    jupyter notebook challenge_rocketpy.ipynb
    ```

**Autor:** Alex dos Santos Burdelis
