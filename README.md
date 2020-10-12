# Exemplo Bot

Bot de exemplo feito em Rasa com o conteúdo do [Rasa PT-BR Boilerplate](https://github.com/lappis-unb/rasa-ptbr-boilerplate). O objetivo desse bot é para ser um projeto simples de introdução ao framework do Rasa e como utilizá-lo.

## Instalação
### Python
É necessário ter o python instalado, recomenda-se a versão `3.7.5` que foi a versão utilizada na criação desse projeto.

**OBS.:** É boa prática utilizar de *virtual envs* para projetos em python, dessa forma os ambientes e bibliotecas ficam devidamente encapsulados.

### Rasa
Para esse projeto foi utilizado o Rasa na versão `1.10.14`. Para baixa-lo execute o comando:

``` bash
pip install rasa==1.10.14
```

## Rode o bot

Para rodar o bot é necessário treiná-lo primeiro, para isso rode os seguites comandos:

``` bash
rasa train nlu
rasa train
```

Com o chatbot devidamente treinado, veja sua interação pelo terminal com o comando:

```
rasa shell
```

## Arquivos do Rasa

Veja um pouco como funciona a separação de arquivos no rasa:

`data/nlu.md` - Contém as **intents**, que serão treinadas pelo NLU para a interpretação da fala do usuário.

`data/stories.md` -  Contém as **stories**, histórias a serem seguidas pelo bot.

`domain.yml` - Contém as **utters**, as respostas do chatbot

`config.yml` - Configurações de treinamento do bot

`tests/conversation_tests.md` - Teste das histórias

`actions.py` - Arquivo para criar ações customizadas, como conecxões a APIs, cálculos e etc.

## Referências

1. [Rasa Docs](https://rasa.com/docs/rasa/)

1. [Financial Services Example Bot](https://github.com/RasaHQ/financial-demo)

1. [Rasa PT-BR Boilerplate](https://github.com/lappis-unb/rasa-ptbr-boilerplate)