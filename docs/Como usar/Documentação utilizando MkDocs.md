# Documentação utilizando MkDocs

Para documentação completa visitar [mkdocs.org](https://www.mkdocs.org).

## Configuração

Visitar [https://www.mkdocs.org/user-guide/configuration/](https://www.mkdocs.org/user-guide/configuration/) para informações sobre a configuração do `mkdocs.yml`

## Comandos

Utilização básica com o ReadTheDocks pode ser vista [aqui](https://docs.readthedocs.io/en/stable/intro/getting-started-with-mkdocs.html)

* `mkdocs new [dir-name]` - Cria um novo projeto.
* `mkdocs serve` - Start the live-reloading docs server.
* `mkdocs build` - Build the documentation site.
* `mkdocs -h` - Print help message and exit.


## Layout do projeto

    mkdocs.yml    # Arquivo de configuração.
    docs/
        index.md  # Pagina inicial da documentação.
        ...       # Outras páginas de markDown, imagens e outros arquivos.


## Temas

[Documentação temas MkDocs](https://www.mkdocs.org/user-guide/choosing-your-theme/)

Por padrão o MkDocs inclui os seguinte temas:
1. mkdocs
2. readthedocs

Temas de terceiros podem ser instalados [aqui](https://github.com/mkdocs/mkdocs/wiki/MkDocs-Themes)

Para escolher um tema altere o arquivo `mkdocs.yml`
```yml
theme:
    name: mkdocs
    nav_style: dark
```
