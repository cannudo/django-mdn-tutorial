# django-mdn-tutorial
Repositório que armazena o código gerado ao ler as docs do MDN, ensinando a usar Django.

## Repositório original
Você pode acessar o repositório original [clicando aqui.](https://github.com/mdn/django-locallibrary-tutorial)

## Instalação

Para rodar o servidor localmente, siga os passos:
1. Configure o [ambiente de desenvolvimento Python](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/development_environment).
   Recomenddamos utilizar um ambiente de desenvolvimento virtual
1. Assumindo que você já tenha o Python configurado na sua máquina, rode os seguintes comandos (se você está utilizando o Windows, talvez precise usar `py` ou `py -3` ao invés de `python` para iniciar o Python):
   ```
   pip3 install -r requirements.txt # Instala as dependências
   python3 manage.py makemigrations # Cria os arquivos de migração
   python3 manage.py migrate # Execeuta os arquivos de migração
   python3 manage.py collectstatic # Reúne os arquivos estáticos para produção
   python3 manage.py test # Run the standard tests. These should all pass.
   python3 manage.py createsuperuser # Cria o superusuário
   python3 manage.py runserver # Roda o servidor
   ```
1. Abra um navegador em `http://127.0.0.1:8000/admin/` para abrir o site administrativo
1. Crie alguns objetos de teste de cada tipo
1. Abra `http://127.0.0.1:8000` para ver seu site, com os objetos recém-criados