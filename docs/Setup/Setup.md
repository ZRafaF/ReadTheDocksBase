# Setup

## Recomendações

É recomendado criar um `venv` para este projeto
`python -m venv venv`

e para ativar

___

:simple-windows: Windows

`venv\Scripts\activate`
    
___

:simple-linux: Linux

`source venv\bin\activate`

___

## Instalando dependências

1. MkDocs
    `pip install MkDocs`

2. Plugin
    Siga as instruções em [Plugins](./Plugins.md) para a instalação dos plugins necessários.

3. Tema
    Siga as instruções em [Temas](./Temas.md) para a instalação do tema utilizado.

## Configuração

Para a configuração mais recente por favor veja o *commit* mais atual [aqui](https://github.com/ZRafaF/ReadTheDocksBase/blob/main/mkdocs.yml)

ou copie o seguinte código possivelmente **DEFASADO**

``` yaml
site_name: Projeto base

repo_url: https://github.com/ZRafaF/ReadTheDocksBase

theme:
    name: material

    palette:
        scheme: slate
        primary: indigo
        accent: indigo

    locale: pt_BR
    features:
        - navigation.sections
        - navigation.tabs
        - navigation.top
        - navigation.tracking
        - navigation.path
        - navigation.indexes
        - search.highlight
        - search.share
        - search.suggest
        - toc.follow
        - content.code.copy

plugins:
    - search:
        separator: '[\s\-,:!=\[\]()"`/]+|\.(?!\d)|&[lg]t;|(?!\b)(?=[A-Z][a-z])'
    - with-pdf:
        author: Rafael Farias
    - pdf-export

markdown_extensions:
    - pymdownx.highlight:
        anchor_linenums: true
        use_pygments: true
        auto_title: true

    - pymdownx.inlinehilite
    - pymdownx.snippets
    - pymdownx.superfences
    - pymdownx.critic
    - pymdownx.caret
    - pymdownx.keys
    - pymdownx.mark
    - pymdownx.tilde
```

## Utilização

Visite a tab [Como usar](/docs/Como_usar/Como_usar.md) para instruções de **utilização** e ***deployment***.