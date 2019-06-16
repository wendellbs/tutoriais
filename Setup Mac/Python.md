# Setup Ambiente Python para Mac

Configurando ambiente Python no MacOS.


## Instalação

    brew install pyenv
    brew install pyenv-virtualenv
    brew install pyenv-virtualenvwrapper

## Criação dos repositórios

    # Todos meus virtualenvs ficam em...
    mkdir ~/.ve
    # Todos meus projetos ficam em...
    mkdir ~/workspace

## Comandos pyenv
* **Instalar versões Python**

    ```
    pyenv install 3.6.8
    pyenv install 2.7.16
    ```

* **Listar versões disponíveis**

    ```
    pyenv install -l
    ```

* **Remover versões**

    ```
    pyenv uninstall 2.7.10
    ```

# Virtualenv
## Pyenv virtualenv

* **Criar virtualenv**
pyenv virtualenv [python version] [nome do virtualenv]

    ```
    pyenv virtualenv 3.7.3 tools3
    ```

* **Ativar virtualenv**
	```
	pyenv activate tools3
	```

* **Desativar virtualenv**
	```
	pyenv deactivate
	```

* **Listar virtualenvs criados**
    ```
    pyenv virtualenvs
    ```

* **Remover virtualenv**
   ```
  pyenv uninstall tools3
  ```

## Pyenv Virtualenv Wrapper
* **Escolhendo versão python local**
pyenv local [python version]

	```
	pyenv local 2.7.16
	```

* **Criar projeto e virtualenv**
Cria o virtualenv `~/.ve/proj3` e a pasta do projeto `~/workspace/proj3` com a versão local de python.

	```
	mkproject proj3
	```

* **Criar virtualenv no repositório atual**
	```
	mkvirtualenv -a $(pwd) tools3
	```

* **Ativar virtualenv**
	```
	workon tools3
	```

* **Desativar virtualenv**
	```
	deactivate
	```

* **Listar virtualenvs criados**
	```
	lsvirtualenv
	```

* **Remover virtualenv criado**
	```
	rmvirtualenv tools3
	```
# Referências
* [Guia definitivo para organizar meu ambiente Python](https://medium.com/welcome-to-the-django/guia-definitivo-para-organizar-meu-ambiente-python-a16e2479b753)
* [pyenv](https://github.com/pyenv/pyenv)
* [pyenv-virtualenv](https://github.com/pyenv/pyenv-virtualenv)
* [pyenv-virtualenvwrapper](https://github.com/pyenv/pyenv-virtualenvwrapper)
* [virtualenvwrapper](https://virtualenvwrapper.readthedocs.io/en/latest/command_ref.html)
