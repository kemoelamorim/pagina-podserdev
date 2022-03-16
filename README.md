# essential-html-css

Estrutura e conceitos básicos de HTML e CSS
> Criação de uma página web

- Tags html
- Propriedades CSS
- Texto
- Imagem
- Blocos de conteúdo
- Lista de informações
- Backgroud color, fontes
- Posicionamento e espaçamento
- Paginação
- Importação de arquivos externos
- Inserção de Videos e maps
- Media queries

>Arquivo index.html
---

É o nome do arquivo principal da página, todo arquivo html deve ser salvo com a extensão html, "index.html" com essa extensão o navegador já consegue mostrar o conteudo do arquivo.

> Tags
---
Uma tag é a anotação semantica para indicar ao navegador a estrutura para da página html.
**Níveis de Títulos**

```
<h1>Título h1</h1>
<h2>Título h2</h2>
<h3>Título h3</h3>
<h4>Título h4</h4>
<h5>Título h5</h5>
<h6>Título h6</h6>
```

<h1>Título h1</h1>
<h2>Título h2</h2>
<h3>Título h3</h3>
<h4>Título h4</h4>
<h5>Título h5</h5>
<h6>Título h6</h6>

`Algumas tags podem tem somente abertura, com o caso da tag <meta> ou <link>, outras podem ter abertura e fechamento e o conteudo entre as tags ex: <h1>conteúdo</h1>`

---

**Parágrafo**

```
<p>Tag que representa um parágrado.</p>
```

Resultado HTML:<p>Tag que representa um parágrado.</p>

---

**Importância Semântica**

Marca o conteúdo como um nível de importancia (não é uma mudança visual, mas sim semântica)

```
<p>Este conteúdo não tem nenhum nível de importancia semântica.<strog> Conteúdo semânticamente importânte</strong>.</p>
```

Resultado HTML:
<p>Este conteúdo não tem nenhum nível de importancia semântica.<strong> Conteúdo semânticamente importânte</strong>.</p>

---

**Enfase no conteúdo**

```
<p>Este conteúdo não tem nenhum nível de importancia semântica.
<strog>Conteúdo semânticamente importânte</strong>. 
<em>Aqui temos uma ênfase no conteúdo</em></p>
```

Resultado HTML:
<p>Este conteúdo não tem nenhum nível de importancia semântica.<strong> Conteúdo semânticamente importânte</strong>. <em>Aqui temos uma ênfase no conteúdo</em></p>

---

### Tags de metadados do Arquivo HTML

> Declarando o tipo do Arquivo:

```
<DOCTYPE hmtl>
```

`A Tag acima identifica o tipo do arquivo para o navegador, neste caso estamos declarando que o arquivo é do tipo hmtl5, que é a versão mais nova do html`

- É importante cocar todas as outra tags da página encapsulada um uma tag html:
  
  ```
    <DOCTYPE html>
    <html>
    ...outras tags...
    </html>
  ```

> Tag head com meta dados e informações de configurações

`A tag <head> passa as informações para o navegador conheca as propriedades da página carregada`

```
<DOCTYPE html>
<html>
    <head>
    ...meta dados...
    </head>
</html>
```

> Declarando o conjunto de caracteres UTF- 8 com a Tag meta e língua pt-br

`Para a página indentificar os caracteres de outras línguas, devemos passar essa informação com para o navegador`

```
<DOCTYPE html>
<html lang="pt-br">
    <head>
        <meta charset="UTF-8">
        <title>Nome da página</title>
    <head>
</html>

```

`A tag meta acima recebe um propriedade charset com o tipo UTF-8 , que informa o navegador o conjuto de caractere usado na página`

---
> Contúdo da página

`O conteúdo da página deve ser colocado entre as tegs body pois é o corpo da página`

```
<DOCTYPE html>
<html lang="pt-br">
    <head>
        <meta charset="UTF-8">
        <title>Nome da página</title>
    <head>
    <body>
        <p>Este conteúdo não tem nenhum níve de importancia semântica.
        <strong> Conteúdo semânticamente importânte</strong>. 
        <em>Aqui temos uma ênfase no conteúdo</em>
        </p>
    </boby>
</html>

```

---
> CSS (Cascate Style Sheet)

`O css significa folha de style em cascata (misturnado inglês com português), e nos permite criar estilos visuais para o arquivo html`
- Existem três formas de usar o css:
    - Em linha: CSS inline
        ``` 
            <p style="font-size: 20px;">
                Texto com tamanho da fonte de 20px
            </p>
        ```

    - Na tag head:
        ```
            <html lang="pt-br">
            <head>
                <style>
                    p {
                        fonte-size: 20px
                    }
                </style>
            <head>
            <body>
                <p>Conteúdo com 20px</p>
            </boby>
            </html>
        ```
    - Em arquivo externo sendo importado no head: usando um arquivo style.css (.css é a extenão assim como o .html)
        ```
            <html lang="pt-br">
            <head>
                <link rel="stylesheet" href="style.css>
            <head>
            <body>
                <p>Conteúdo com 20px</p>
            </boby>
            </html>
        ```