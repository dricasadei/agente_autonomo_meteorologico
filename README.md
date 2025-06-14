# Agente Autônomo de Alerta Climático

O agente conforme as 10 últimas medições de indicativos climaticos avalia e decide se deve enviar um email alertando de possibilidade de tempestades.

## Como rodar a aplicação

- python create_db.py 
    - para criar a estrutura do banco de dados que receberá as informações climáticas.

- python weather_api.py | python weather_api.py --storm 
    - duas formas de inicializar a api, sem parâmentro indica que os dados criados artificialmente sobre o clima terão pouca variação. Se for incluido o parâmentro --storm os dados gerados terão uma variabilidade maior e o modelo ao analisar, pode entender que terá a necessidade de envio de email de alerta.

- python weather_agent.py
    - inicializa o agente para ficar verificando os dados climáticos e avaliando a necessidade de envio de email de alerta.
