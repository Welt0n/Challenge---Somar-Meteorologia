# Challenge---Somar-Meteorologia
API para o desafio da Somar Meteorologia

Esta é a uma versão inicial. 


Próximos passos inclui :


  Endpoint para consulta de estações e periodos disponíveis
  
  
  Endpoint para pesquisa de multiplas estações
  
  
  GraphQL
  
  
  Testes 
  
  
  




Basta montar um repositório com app.py, consumer.py e a pasta 'data' do repositório https://github.com/somarmeteorologia/challenge/tree/master/backend
Rodar app.py. E então fazer os requests. As variaveis requeridas são :


  station, latitude, longidute => Usadas para a identificação da tabela.
  
  
  A API prioriza station e caso decida usar latitude, longitude, ela irá encontrar a estação mais proxima à coordenada dada.
  
  
  init_date, final_date, days => Usadas para definir o periodo.
  
  
  A API prioriza init_date e final_date caso dado. Formato da data é como em : 2019-08-12, "%Y-%m-%d"
  
  
  Os periodos disponíveis para consulta são : 
  
  
    Dados observados : De 2019-08-12 à 2019-09-10.
    
    
    Dados de previsão : De 2019-09-11 à 2019-10-10.
    
    
    A data atual é definida como 2019-09-11 de acordo com os dados.
    
    

Exemplos de request:

http://localhost:5000/observed?station=Alegria-MG&days=10

http://localhost:5000/observed?init_date=2019-08-16&final_date=2019-08-18&latitude=-16.08&longitude=-48.50

http://localhost:5000/forecast?init_date=2019-09-12&final_date=2019-09-16&latitude=-16.08&longitude=-48.5

http://localhost:5000/forecast?days=10&latitude=-16.08&longitude=-48.5


