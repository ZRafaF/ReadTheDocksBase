# MkDocs Setup

## Recomendações

É recomendado criar um `venv` para este projeto
`python -m venv venv`

e para ativar
`venv\Scripts\activate`

## Instalando dependências

MkDocs
`pip install MkDocs`

### Plug-ins

mkdocs-with-pdf [repo](https://github.com/orzih/mkdocs-with-pdf)

`pip install mkdocs-with-pdf`

Habilitando o plugin no `mkdocs.yml`
``` yml
plugins:
    - with-pdf
```

Os parâmetros de configuração podem ser encontrados [aqui](https://github.com/orzih/mkdocs-with-pdf#configuration)

O arquivo pode ser encontrado em 
### [pdf](../pdf/document.pdf)

> **note**

Seu path é `pdf/document.pdf`

### Temas

O tema escolhido para essa documentação é [mkdocs-rtd-dropdown](https://github.com/cjsheets/mkdocs-rtd-dropdown), este deve ser instalado manualmente.

`pip install mkdocs-rtd-dropdown`

Habilitando o tema no `mkdocs.yml`
``` yml
theme:
    name: rtd-dropdown
```

Outro tema bastante completo e bonito é o [Materials for MkDocs](https://squidfunk.github.io/mkdocs-material/)