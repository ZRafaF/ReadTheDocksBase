# Deploying

Para realizar o *deployment* no github-pages temos algumas opções diferentes.

## gh-deploy

Fazemos uma build direto na *branch* `gh-deploy`. Essa tarefa pode ser feita manualmente com o comando
`mkdocs gh-deploy --force`

ou automaticamente com o GitHub Actions. Ver [https://squidfunk.github.io/mkdocs-material/publishing-your-site/](https://squidfunk.github.io/mkdocs-material/publishing-your-site/).

## Manualmente

Para fazer o *deployment* manualmente precisamos definir o diretório `docs` como o `site_dir` do MkDocs, e aplicar setar a github page para esse endereço.

Começamos adicionando a seguinte linha ao arquivo `mkdocs.yml` 

``` yaml
docs_dir: 'docsSrc'
site_dir: 'docs'
```

Note que agora o **código fonte** está localizado no diretório `docsSrc` e o ***output*** no diretório `docs`.

Podemos então realizar uma *build* manual com o comando

`mkdocs build`