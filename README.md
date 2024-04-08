# Flask

Flask é um framework de baixo nível [WSGI][] para aplicações web. Ele foi
desenhado para ter uma iniciação rápida e fácil, com a habilidade de escalar
para aplicações complexas. Começou como um wrapper simples entre [Werkzeug][]
e [Jinja][], e se tornou um dos mais populares frameworks para desenvolvimento
web em Python.

Flask oferece sugestões, mas não impõe qualquer dependência ou
layout de projeto. Está na mão dos desenvolvedores a escolha de quais
ferramentas e bibliotecas querem utilizar. Existem diversas extensões
disponibilizadas pela comunidade que facilita a adição de novas
funcinoalidades.

[WSGI]: https://wsgi.readthedocs.io/
[Werkzeug]: https://werkzeug.palletsprojects.com/
[Jinja]: https://jinja.palletsprojects.com/


## Instalando

Instale e atualize pelo [PyPI][] utilizando um instalador como o [pip][]:

```
$ pip install -U Flask
```

[PyPI]: https://pypi.org/project/Flask/
[pip]: https://pip.pypa.io/en/stable/getting-started/


## Exemplo simples

```python
# Salve isso como app.py
from flask import Flask

app = Flask(__name__)

@app.route("/")
def ola_mundo():
    return "Olá, Mundo!"
```

```
$ flask run
  * Running on http://127.0.0.1:5000/ (Press CTRL+C to quit)
```


## Contribuindo

For guidance on setting up a development environment and how to make a
contribution to Flask, veja o [guia de contribuição][].

[guia de contribuição]: https://github.com/pallets/flask/blob/main/CONTRIBUTING.rst


## Doação

The Pallets organization develops and supports Flask and the libraries
it uses. In order to grow the community of contributors and users, and
allow the maintainers to devote more time to the projects, [please
donate today][].

[please donate today]: https://palletsprojects.com/donate
