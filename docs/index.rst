.. rst-class:: hide-header

Bem vindo ao Flask
==================

.. image:: _static/flask-horizontal.png
    :align: center

Bem vindo a documentação do Flask. Flask um framework de baixo nível WSGI para aplicações web.
Ele foi desenhado para ter uma iniciação rápida e fácil, com a habilidade de escalar
para aplicações complexas.

Comece com :doc:`installation`
e tenha uma visão geral em :doc:`quickstart`. Há tambéum uma apresentação
mais detalhada :doc:`tutorial/index` que mostra como criar uma pequena
aplicação completa com Flask. Padrões comuns estão descritos na seção
:doc:`patterns/index`. O restande da documentação descreve os detalhes de cada
componente do Flask, com uma referência completa na seção :doc:`api`.

Flask depende do `Werkzeug`_ WSGI toolkit, o `Jinja`_ template engine, e o
`Click`_ CLI toolkit. Cheque também suas documentações além da documentação do
Flask quando buscar informações.

.. _Werkzeug: https://werkzeug.palletsprojects.com
.. _Jinja: https://jinja.palletsprojects.com
.. _Click: https://click.palletsprojects.com


Guia de usuário
---------------

Flask fornece configurações e convenções, com padrões claros, para iniciar.
Essa seção da documentação explica as diferentes partes do framework Flask e como
as utilizar, customizar e expandir. Para além do próprio Flask, veja as extenções
desenvolvidas pela comunidade para adicionar ainda mais funcionalidades.

.. toctree::
   :maxdepth: 2

   installation
   quickstart
   tutorial/index
   templating
   testing
   errorhandling
   debugging
   logging
   config
   signals
   views
   lifecycle
   appcontext
   reqcontext
   blueprints
   extensions
   cli
   server
   shell
   patterns/index
   web-security
   deploying/index
   async-await


Referência da API
-----------------

Se estiver buscando informações sobre uma função, classe ou método específico,
essa parte da documentação é para você.

.. toctree::
   :maxdepth: 2

   api


Notas adicionais
----------------

.. toctree::
   :maxdepth: 2

   design
   extensiondev
   contributing
   license
   changes
