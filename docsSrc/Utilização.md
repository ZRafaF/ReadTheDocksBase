# Utilização

## Criando páginas e sub-páginas
Para criar uma nova página deverá ser criado um novo documento `.md` na pasta `docs`. Este documento será automaticamente *linkado* ao projeto, e o seu nome será adicionado ao inxador. 


A itens e sub-itens é feita utilizando o `#` quanto maior a quantidade de *nested* `#` maior a subdivisão.

Exemplo de sintaxe
```markdown
# Principal         <!-- Cria um novo tópico, não é recomendado a criação de mais de um tópico por página -->
Esse texto está presente na pagina "Principal"

## Item_A           <!-- Cria um item chamado "Item_A" na página "Principal" -->
Esse texto está presente no "Item_A"

### Como cozinhar   <!-- Cria um sub-item no item "Item_A" -->
Esse texto está presente no sub-item "Como cozinhar"

## Item_B           <!-- Cria um item chamado "Item_B" na página "Principal" -->

```

## Sintaxe básica

MkDocs faz uso dos comandos da linguagem de marcação MarkDown, ver [Sintaxe básica de MarkDown](https://www.markdownguide.org/basic-syntax/)

* `*texto*` *Texto em itálico*
* `**texto**` **Texto em bold**
* ``` `texto` ``` `Código em linha`

___

## Sintaxe estendida
Alguma das funções estendidas também funcionam com o MkDocs, ver [Sintaxe estendida](https://www.markdownguide.org/extended-syntax/)

### Código
` ``` ` Código vai aqui ` ``` `

```
//Múltiplas linhas de código

void max()
{
    
}
```

Também podemos indicar qual linguagem estamos utilizando, o *sintaxe highlighter* utilizado é o **highlight.js** a lista de linguas suportadas pode ser encontrada [aqui](https://github.com/highlightjs/highlight.js/blob/main/SUPPORTED_LANGUAGES.md).

` ```cpp ` int main()... ` ``` `



Tambem será necessário adicionar essa lingua extra "Extensão" ao arquivo `mkdocs.yml`

```
    hljs_languages:
        - cpp
        - md
```

___

### Linhas

* `___` Cria uma linha de separação
> ___
___

### Citação

* `>` Cria uma citação
> Citação

___

### Tabelas

``` md
| Syntax      | Description |
| ----------- | ----------- |
| Header      | Title       |
| Paragraph   | Text        |
```

| Syntax      | Description |
| ----------- | ----------- |
| Header      | Title       |
| Paragraph   | Text        |

___

### Imagens

Um breve tutorial sobre a inserção de imagens pode ser encontrada [aqui](https://marinegeo.github.io/2018-08-10-adding-images-markdown/).

Sintaxe
`![Nome da imagem](caminho da imagem)`

exemplo

`![Exemplo de imagem](exemploImagem.png)`

![Exemplo de imagem](exemploImagem.png)

___

### Linkando outra página ou item

A documentação oficial pode ser encontrada [aqui](https://www.mkdocs.org/user-guide/writing-your-docs/)

* Exemplo de link para outra página da documentação `[Documentação utilizando MkDocs](./index.md)` [Documentação utilizando MkDocs](./index.md)


* Exemplo de link para outro item `[sintaxe-básica](./Utilização.md#sintaxe-basica)` [sintaxe-básica](./Utilização.md#sintaxe-basica)
> Importante notar que a URL não deve conter acentuação
___


