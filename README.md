# Machine Learning com Azure ML

Este repositório detalha a criação de um modelo de previsão utilizando o Azure Machine Learning. 

## Links Úteis

- Explore os [Serviços de IA do Azure](link_para_exploracao_ai_azure)
- Conheça o [Machine Learning Automatizado no Azure Machine Learning](link_para_ml_automatizado_azure_ml)
- Fonte dos dados: [Link para os dados](link_para_fonte_dados)

## Passo 1: Criando Recurso no Azure Machine Learning

- Clique em "Criar recurso" e busque por "Azure Machine Learning".
- Preencha os detalhes, como "Resource group", "Name" e "Region", mantendo padrões sugeridos.
- Após a criação, vá para o recurso.

## Passo 2: Configuração do Recurso

- Preencha os campos do workspace, como "Resource group", "Name", e "Region".
- Crie o recurso e clique em "ir para recurso".

## Passo 3: Configuração do Trabalho de ML Automatizado

- No menu lateral, clique em "ML automatizado" e depois em "Novo trabalho de ML automatizado".
- Em "Configurações básicas", preencha "Nome do trabalho" e "Novo nome do experimento".
- Selecione "Regressão" como tipo de tarefa e configure os dados.
- Escolha a fonte de dados, informando a URL para o treinamento do modelo.
- Configure as demais opções conforme necessário.
- Após o carregamento dos dados, clique em "criar".

## Passo 4: Métricas do Modelo

- Acesse as métricas do modelo treinado na página do modelo, utilizando o link fornecido em "Criado por trabalho".
- Alternativamente, acesse o trabalho na opção do menu "Tarefas (jobs)" e navegue até a aba de métricas.

## Passo 5: Teste do Modelo

- Na página do modelo, clique na aba "Pontos de extremidade" ou acesse pelo menu lateral em "Pontos de extremidade".
- Selecione o ponto correspondente ao modelo gerado e vá para a aba "Testar".
- Realize o teste utilizando o JSON fornecido.

## Dados de Teste JSON

```json
{
  "input_data": {
    "data": [
       {
         "day": 1,
         "mnth": 1,   
         "year": 2022,
         "season": 2,
         "holiday": 0,
         "weekday": 1,
         "workingday": 1,
         "weathersit": 2, 
         "temp": 0.3, 
         "atemp": 0.3,
         "hum": 0.3,
         "windspeed": 0.3 
       }
     ]
  }
}
