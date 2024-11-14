# aluguel-bike
# Automação de Previsão de Aluguéis de Bicicletas com Azure Machine Learning 🚲

Neste projeto, vamos automatizar a previsão de **aluguel de bicicletas** utilizando o **Azure Machine Learning (Azure ML)**. Com dados locais de um arquivo CSV, conseguimos analisar e prever o número de aluguéis com base em variáveis como temperatura, umidade, hora do dia e outros fatores que influenciam a demanda por bicicletas.

Aqui você vai encontrar o passo a passo de como montamos essa automação, desde a preparação dos dados até o treinamento do modelo e a criação da pipeline de automação no Azure.

## Índice

1. [Configuração Inicial](#1-configuração-inicial)
2. [Carregamento e Pré-processamento de Dados](#2-carregamento-e-pré-processamento-de-dados)
3. [Criação e Treinamento do Modelo de Machine Learning](#3-criação-e-treinamento-do-modelo-de-machine-learning)
4. [Automação com Azure ML Pipeline](#4-automação-com-azure-ml-pipeline)
5. [Acompanhamento e Execução de Testes](#5-acompanhamento-e-execução-de-testes)
6. [Conclusão](#6-conclusão)

---

## 1. Configuração Inicial

Antes de começarmos, precisamos garantir que o ambiente de trabalho no **Azure Machine Learning** esteja pronto e que todas as dependências estejam instaladas.

### 1.1. Criar uma Conta no Azure

Se você ainda não tem uma conta no **Azure**, basta ir até o [Portal do Azure](https://portal.azure.com/) e criar uma. A Azure tem planos gratuitos para iniciantes, então você pode começar sem compromisso.

### 1.2. Criar um Workspace no Azure ML

Depois de criar sua conta, o próximo passo é criar um **Workspace** no **Azure Machine Learning**. O Workspace será o lugar onde vamos gerenciar todos os nossos experimentos, modelos e recursos de computação. É como se fosse a "central de comando" do nosso projeto.

### 1.3. Instalar o SDK do Azure ML

Agora, vamos instalar o SDK do **Azure Machine Learning** no seu ambiente local para interagir com o Azure de dentro do código Python. Execute o seguinte comando no seu terminal:

```bash
pip install azureml-sdk
