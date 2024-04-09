Instalação
==========


Versão do Python
----------------

Nós recomendamos utilizar a última versão do Python. Flask suporta Python 3.8 e mais recentes.


Dependências
------------

Essas distribuições vão ser instaladas automaticamente com o Flask.

* `Werkzeug`_ implementa WSGI, a interface padrão do Python entre
  aplicações e servidores.
* `Jinja`_ é uma linguagem de template que renderiza as páginas da sua aplicação.
* `MarkupSafe`_ vem com o Jinja. Desvia de inputs não confiávevis enquanto
  renderiza templates, para evitar ataques de injeção.
* `ItsDangerous`_ assina dados seguros para garantir sua integridade. É usado
  para proteger os cookies da sessão no Flask.
* `Click`_ é um framework para aplicações de linhas de comando. Fornece o comando
   ``flask`` e permite adicionar comandos de gerenciamento customizados.
* `Blinker`_ fornece suporte para o :doc:`signals`.

.. _Werkzeug: https://palletsprojects.com/p/werkzeug/
.. _Jinja: https://palletsprojects.com/p/jinja/
.. _MarkupSafe: https://palletsprojects.com/p/markupsafe/
.. _ItsDangerous: https://palletsprojects.com/p/itsdangerous/
.. _Click: https://palletsprojects.com/p/click/
.. _Blinker: https://blinker.readthedocs.io/


Dependências opcionais
~~~~~~~~~~~~~~~~~~~~~~

Essas distribuições não serão instaladas automaticamente. Flask vai detectá-las
e utilizá-las caso você as instale.

* `python-dotenv`_ habilita suporte para :ref:`dotenv` enquanto roda comandos
  ``flask``.
* `Watchdog`_ fornece um reloader mais rápido e mais eficiente para servidores
  de desenvolvimento.

.. _python-dotenv: https://github.com/theskumar/python-dotenv#readme
.. _watchdog: https://pythonhosted.org/watchdog/


greenlet
~~~~~~~~

Talvez você opte por usar gevent ou eventlet com sua aplicação. Nesse caso, 
será necessário greenlet>=1.0. Quando utilizar PyPy, PyPy>=7.3.7 será
necessário.

Essas não são versões mínimas suportadas, apenas indicam as primeiras versões
que adicionaram features necessárias. Você deverá usar a última versão de cada.


Ambientes virtuais
------------------

Use ambiente virtual para gerenciar as dependências do seu projeto, em 
desenvolvimento e em produção.

Quais problemas o ambiente virtual resolve? Quanto mais projetos em Python você
tiver, mais provável que você necessite usar diferentes versões de bibliotecas
Python, ou do próprio Python. Novas versões de bibliotecas utilizadas em um
projeto podem quebrar a compatibilidade de outro.

Ambientes virtuais são grupos independentes de bibliotecas Python, um para cada 
projeto. Pacontes instalados para um projeto não vão afetar outros projetos ou 
os pacotes do sistema operante.

Python já vem com o módulo :mod:`venv` para criar ambientes virtuais.


.. _install-create-env:

Crie um ambiente
~~~~~~~~~~~~~~~~

Cria uma pasta para o projeto e uma pasta :file:`.venv` utilizando:

.. tabs::

   .. group-tab:: macOS/Linux

      .. code-block:: text

         $ mkdir myproject
         $ cd myproject
         $ python3 -m venv .venv

   .. group-tab:: Windows

      .. code-block:: text

         > mkdir myproject
         > cd myproject
         > py -3 -m venv .venv


.. _install-activate-env:

Ative o ambiente
~~~~~~~~~~~~~~~~

Antes de trabalhar no seu projeto, ative o ambiente correspondente:

.. tabs::

   .. group-tab:: macOS/Linux

      .. code-block:: text

         $ . .venv/bin/activate

   .. group-tab:: Windows

      .. code-block:: text

         > .venv\Scripts\activate

Seu shell prompt vai mudar para mostrar o nome do ambiente virtual ativado.


Instale o Flask
-------------

Com o ambiente ativado, use o seguinte comando para instalar o Flask:

.. code-block:: sh

    $ pip install Flask

Flask agora está instalado. Cheque o :doc:`/quickstart` ou vá para o
:doc:`Documentation Overview </index>`.
