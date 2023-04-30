
# Consulta-Rejeicoes-SEFAZ

Este projeto é um fork do projeto de https://github.com/gabrieellimapy/Consulta-Rejeicoes-SEFAZ, com intuito de aprendizado da integração com o openai, e indo um pouco mais e integrando com https://github.com/python-telegram-bot/python-telegram-bot, com a ideia de fazer um bot ao qual recebe um codigo de rejeição do SEFAZ, faz a pesquisa da solução no chatgpt e traz a possivel resposta para o usuario.


## Autores

- [@mukasc](https://www.github.com/mukasc)


## Instalação

Como sugestão é possivel rodar o projeto utilizando o : https://colab.research.google.com/

Instale o projeto com pip

```bash
  pip install openai 
  pip install nest_asyncio 
  pip install python-telegram-bot --upgrade 
  pip install python-telegram-bot[all] 
  pip install python-telegram-bot[ext]
```
Foi utilizado uma maquina no google colab para os testes a biblioteca nest_asyncio foi utilizada para suprir um erro de loop de threads, não entendi se é por causa do computador compartilhado ou outro coisa, talvez possa ser melhorado.

A pasta com o arquivo csv pode ser que seja data ou sample data(usada no computador colab).

A pasta config e o arquivo config.ini devem ser criados(caso googlecolab) ou alterados inserindo os respectivos tokens da Openai e do Telgram na área testing do arquivo, são necessarios para a utilização dos servições.

```
[DEFAULT]
DB_NAME = db_name_default
DB_USER = db_user_default
DB_PASSWORD = db_password_default
TOKENBOT = tokenbot_default
TOKENOPENAI = tokenopenai_default
[TESTING]
DB_NAME = db_name_testing
DB_USER = db_user_testing
DB_PASSWORD = db_password_testing
TOKENBOT = tokenbot_testing
TOKENOPENAI = tokenopenai_testing
[PRODUCTION]
DB_NAME = db_name_production
DB_USER = db_user_production
DB_PASSWORD = db_password_production
TOKENBOT = tokenbot_production
TOKENOPENAI = tokenopenai_production
```
## Licença

[MIT](https://choosealicense.com/licenses/mit/)

