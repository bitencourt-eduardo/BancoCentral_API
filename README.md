# API ACESSO IPCA BANCO CENTRAL: <h1>

O exercício a ser desenvolvido para a presente unidade consiste em conectar-se a uma API. 
O Banco Central do Brasil disponibiliza dados a respeito de diversos indicadores econômicos do país. 
Sua tarefa será encontrar a série histórica relativa à inflação (IPCA) na plataforma de dados abertos do BC, importá-la e transformá-la em um DataFrame do Pandas.

### API do Banco Central: 
<https://dadosabertos.bcb.gov.br/dataset?res_format=API>

#### Endereço padrão de acesso API:

https://api.bcb.gov.br/dados/serie/bcdata.sgs.{codigo_serie}/dados?formato=json&dataInicial={dataInicial}&dataFinal={dataFinal}

**Parâmetros:**

**codigo_Serie** (obrigatório): parâmetro numérico que representa o código da série a ser consultada.

**dataInicial** (opcional): parâmetro textual que representa a data de início da consulta, no formato dd/MM/aaaa.

**dataFinal** (opcional): parâmetro textual que representa a data final da consulta, no formato dd/MM/aaaa.

O serviço permite também recuperar os N últimos valores de uma determinada série:
        <https://api.bcb.gov.br/dados/serie/bcdata.sgs.{codigo_serie}/dados/ultimos/{N}?formato=json>

### Sistema Gerenciador de Séries Temporais do Bacen (SGS)

https://www3.bcb.gov.br/sgspub/localizarseries/localizarSeries.do?method=prepararTelaLocalizarSeries


Para série IPCA código da sérire: 433 ( Índice nacional de preços ao consumidor-amplo (IPCA) )
