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

Para orientações sobre como configurar um ambiente de desenvolvimento e como
contribuir para o Flask, veja o [guia de contribuição][].

[guia de contribuição]: https://github.com/louipasquini/flask/blob/docs-ptbr/CONTRIBUTING.rst


## Doação

A organização Pallets desenvolve e dá suporte ao Flask e as bibliotecas que
ele utiliza. Para a comunidade de colaboradores e usuários crescer, e
permitir que os mantenedores dediquem mais tempo aos projetos, [por favor, doe hoje][].

[por favor, doe hoje]: https://palletsprojects.com/donate
