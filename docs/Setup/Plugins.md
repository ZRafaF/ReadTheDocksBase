# Plug-ins

## [mkdocs-with-pdf](https://github.com/orzih/mkdocs-with-pdf)

Este plugin gera um arquivo de toda a documentação automaticamente

`pip install mkdocs-with-pdf`

Habilitando o plugin no `mkdocs.yml`
``` yaml
plugins:
    - with-pdf
```

Os parâmetros de configuração podem ser encontrados [aqui](https://github.com/orzih/mkdocs-with-pdf#configuration)

O arquivo pode ser encontrado em baixado [aqui](https://github.com/ZRafaF/ReadTheDocksBase/raw/gh-pages/pdf/document.pdf)

Seu path é `pdf/document.pdf`

!!! tip

    O `mkdocs.yml` deste repositório esta configurado para **apenas exportar se a *environment variable* `ENABLE_PDF_EXPORT` for `1`. caso você queira que os arquivos de PDF sejam gerados com todas as `build` ou `serve` exclua essa opção.

    ``` yaml
    plugins:
    - with-pdf:
        enabled_if_env: ENABLE_PDF_EXPORT # remova essa linha para habilitar o PDF a todo momento
    ```

    > O processo de gerar PDFs tomam tempo considerável, e exportar-los todas as vezes que o programa for executado durante o desenvolvimento acaba atrapalhando. 

___

## [mkdocs-pdf-export-plugin](https://github.com/zhaoterryy/mkdocs-pdf-export-plugin)

Este plugin gera um arquivo em PDF para todas as páginas

`pip install mkdocs-pdf-export-plugin`

Habilitando o plugin no `mkdocs.yml`
``` yaml
plugins:
    - pdf-export
```

!!! tip

    O `mkdocs.yml` deste repositório esta configurado para **apenas exportar se a *environment variable* `ENABLE_PDF_EXPORT` for `1`. caso você queira que os arquivos de PDF sejam gerados com todas as `build` ou `serve` exclua essa opção.

    ``` yaml
    plugins:
    - pdf-export:
        enabled_if_env: ENABLE_PDF_EXPORT # remova essa linha para habilitar o PDF a todo momento
    ```

    > O processo de gerar PDFs tomam tempo considerável, e exportar-los todas as vezes que o programa for executado durante o desenvolvimento acaba atrapalhando. 

___

