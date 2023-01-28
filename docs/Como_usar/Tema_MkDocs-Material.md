# Tema MkDocs-Material

Aqui daremos instruções básicas e referências de como tirar melhor proveito do tema **Materials**.

## Admonition customizado

A criação de novos admonitions é realizada no arquivo `docs/stylesheets/extra.css`:

``` css
/* Criando um admonition chamado admonition-custom */

.md-typeset .admonition.admonition-custom,
.md-typeset details.admonition-custom {
  border-color: rgb(43, 155, 70);
}
.md-typeset .admonition-custom > .admonition-title,
.md-typeset .admonition-custom > summary {
  background-color: rgba(43, 155, 70, 0.1);
}
.md-typeset .admonition-custom > .admonition-title::before,
.md-typeset .admonition-custom > summary::before {
  background-color: rgb(43, 155, 70);
  -webkit-mask-image: var(--md-admonition-icon--admonition-custom);
          mask-image: var(--md-admonition-icon--admonition-custom);
}
```

E por fim definimos seu ícone no arquivo `mkdocs.yml`, para ver uma lista dos `icon` visite [admonition-icons](https://squidfunk.github.io/mkdocs-material/reference/admonitions/#admonition-icons)

``` yaml
theme:
    icon:
        admonition:
            admonition-custom: material/bicycle
```

Por fim utilize com

``` md
!!! admonition-custom

    Eu sou um admonition cutomizado!
```

!!! admonition-custom

    Eu sou um admonition cutomizado!

Para mais referencias visitar a [documentação oficial](https://squidfunk.github.io/mkdocs-material/reference/admonitions/#customization)