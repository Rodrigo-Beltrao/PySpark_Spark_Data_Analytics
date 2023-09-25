# PySpark_Spark_Data_Analytics
Neste projeto, foi feita a análise dos mesmos dados do meu projeto Hadoop (https://github.com/Rodrigo-Beltrao/Hadoop_Hive_GCP) que foi realizado anteriormente com SQL no Hive e agora está sendo feita com PySpark.

<p align="center">
    <img src="https://www.softwebsolutions.com/wp-content/uploads/2016/06/Spark-Hadoop.jpg" alt="Spark">
</p>

## Spark na cloud GCP
Conforme pode ser observado na imagem abaixo, o Spark está devidamente instalado no cluster. No entanto, optei por usar o ambiente Google Colab para realizar as análises com PySpark.

<p align="center">
    <img src="https://i.imgur.com/lOllJhd.png" alt="Spark2">
</p>

## Consultas
Para cada consulta em SQL, foi realizada uma consulta utilizando o PySpark com funções de agregação.

<p align="center">
    <img src="https://i.imgur.com/NThvcAP.png" alt="Spark2">
</p>

## Análises exploratórias
Foram realizadas duas consultas além das realizadas no projeto Hadoop. Essas novas consultas permitiram uma análise exploratória mais detalhada da quantidade de cartões de crédito fraudulentos. Dos 19.936 cartões, apenas 27 são fraudulentos. De acordo com os gráficos abaixo, o número de cartões de crédito fraudulentos representam 0,1% do total de cartões.

<p align="center">
    <img src="https://i.imgur.com/4IyVZKz.png" alt="Spark2">
</p>

### Fonte dos dados:

Kaggle - https://www.kaggle.com/datasets/ealtman2019/credit-card-transactions?select=sd254_users.csv

# Dicionário de Dados

## Tabela: user0_credit_card_transactions

| Coluna                  | Descrição                                       |
|-------------------------|-------------------------------------------------|
| chave                   | Chave única para a transação                    |
| card                    | Número do cartão de crédito utilizado na transação |
| year                    | Ano da transação                                |
| month                   | Mês da transação                                |
| day                     | Dia da transação                                |
| tempo                   | Horário da transação                            |
| amount                  | Valor da transação                              |
| use_chip                | Indica se o chip do cartão foi utilizado       |
| merchant_name           | Nome do estabelecimento comercial               |
| merchant_state          | Estado do estabelecimento comercial             |
| zip                     | Código postal do estabelecimento comercial      |
| mcc                     | Código de categoria do estabelecimento comercial |
| errors                  | Indica se ocorreram erros na transação          |
| is_fraud                | Indica se a transação é fraudulenta             |

## Tabela: sd254_users

| Coluna                  | Descrição                                       |
|-------------------------|-------------------------------------------------|
| person                  | Identificação única da pessoa                  |
| current_age             | Idade atual da pessoa                          |
| retirement_age          | Idade de aposentadoria da pessoa               |
| birth_year              | Ano de nascimento da pessoa                    |
| gender                  | Gênero da pessoa                               |
| address                 | Endereço da pessoa                             |
| apartment               | Número do apartamento da pessoa                |
| city                    | Cidade da pessoa                               |
| state                   | Estado da pessoa                               |
| zipcode                 | Código postal da pessoa                        |
| latitude                | Latitude da localização da pessoa              |
| longitude               | Longitude da localização da pessoa             |
| per_capita_income       | Renda per capita na região do CEP              |
| yearly_income           | Renda anual da pessoa                          |
| total_debt              | Dívida total da pessoa                         |
| fico_score              | Pontuação FICO da pessoa                       |
| num_credit_cards        | Número de cartões de crédito da pessoa         |

## Tabela: sd254_cards

| Coluna                  | Descrição                                       |
|-------------------------|-------------------------------------------------|
| chave2                  | Chave única para o cartão                      |
| card_index              | Índice do cartão                               |
| card_brand              | Marca do cartão                                |
| card_type               | Tipo do cartão                                 |
| card_number             | Número do cartão                               |
| expires                 | Data de expiração do cartão                    |
| cvv                     | Código de segurança do cartão                  |
| has_chip                | Indica se o cartão possui chip                |
| cards_issued            | Número de cartões emitidos para o usuário      |
| credit_limit            | Limite de crédito do cartão                    |
| acct_open_date          | Data de abertura da conta do cartão            |
| year_pin_last_changed   | Ano em que o PIN do cartão foi alterado        |
| card_on_dark_web        | Indica se o cartão está na Dark Web            |
