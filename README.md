# project_m13

        OBS!!!
            O professor instalou o Poetry no ambiente global porem na documentação e explicitamente 
            descrito que ele so deve ser instalado em um ambiente virtual para não haver conflitos 

            - Usando seu ambiente virtual
            
                Por padrão, o Poetry cria um ambiente virtual em {cache-dir}/virtualenvs. Você pode alterar 
                o cache-dirvalor editando a configuração do Poetry. Além disso, você pode usar a 
                virtualenvs.in-projectvariável de configuração para criar ambientes virtuais dentro do diretório do seu projeto.

                https://python-poetry.org/docs/basic-usage/#using-your-virtual-environment

        - Inicie o Poetry e instale as dependencia que você vai usar no projeto    

                poetry init 

                - Vamos instalar 

                    pytest
                    factory-boy

                - Ver as configurações informadas 

                        cat pyproject.toml

            - Quando criamos um venv iniciamos o projeto assim:

                - Inicindo um projeto com o poetry

                    poetry new <nome do projeto>                

        - Instalando o django com o poetry

            poetry add django     

        -  Iniciando um projeto com o poetry/django          

            poetry run django-admin.py startproject <nome do projeto> . 

                (O ponto indica para o django iniciar dentro do diretorio atual)

        - Iniciando o app com o django/poetry

            poetry run python3 manage.py startapp api

        - Rodando a migração    

            poetry run python3 manage.py migrate

        - Testando o setup do projeto 

            poetry run python3 manage.py runserver