## Sync vs Async

Este projeto foi desenvolvido durante as aulas da EBAC com o objetivo de vermos na pratica a diferença de uma view sincrona e assincrona em Django.

O projeto consiste em duas paginas, uma configurada de maneira assincrona e outra configurada de maneira sincrona. <br>
Assim podemos observar o comportamento delas, sendo a sincrona executando toda a linha de codigo antes de devolver a resposta html, em contrapartida a assincrona entrega a resposta html
ao mesmo tempo que resolve a outra parte do codigo.

<br>


### Como executar:
<br>

* Clone o repositório utilizando o seguinte comando:

```bash
$ git clone https://github.com/pauloandrecss/async-views.git
```

* Vamos entrar em nossa pasta do projeto e criar um ambiente virtual:

```bash
$ cd async-views
$ python3 -m venv venv
```

* Agora podemos iniciar nosso ambiente virtual e instalar as bibliotecas necessarias:
  
```bash
$ source venv/bin/activate - Caso utilize linux
$ venv/Scripts/Activate - Caso utilize windows

$ pip install -r requirements.txt
```

* Agora com tudo pronto inicie o servidor utilizando o comando:

```bash
$ uvicorn --reload asyncviews.asgi:application
```
obs: Caso esteja utilizando windows substitua o comando python3 por apenas python.
<br>
<br>
Acesse http://127.0.0.1:8000/async ou http://127.0.0.1:8000/sync e teste o comportamento das diferentes views.
<br>
