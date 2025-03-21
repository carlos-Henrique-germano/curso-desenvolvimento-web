# Guia de Estudo CSS

## Seletores CSS

### Seletor Universal
```css
* {
    border: 1px solid red;
}
```

### Seletor de Texto
```css
h1 {
    color: green;
}
```

### Seletor de Classe
```css
.brown {
    color: brown;
}

p.brown {
    color: brown;
}
```

### Seletor de ID
```css
#header {
    border: 1px solid blue;
}
```

### Seletor de Filho (`>`)
```css
li > a {
    color: red;
    text-decoration: none;
}
li > span {
    color: cyan;
    text-decoration: overline;
    font-size: 2.5em;
}
```

### Seletor de Descendente
```css
p a {
    color: green;
}
```

### Seletor de Irmão Adjacente (`+`)
```css
h1 + p {
    color: darkorange;
    font-size: 32px;
}
```

### Seletor de Irmão Geral (`~`)
```css
h3 ~ p {
    color: hotpink;
    font-size: 24px;
}
```

## Herança e Especificidade
```css
body {
    color: red;
}

p {
    color: blue;
}

p {
    color: green;
}

#page p {
    color: green !important;
}

#page p {
    color: blue;
}
```

## Barras de Navegação

### Barra de Navegação Vertical
```css
ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
}
```

### Barra de Navegação Horizontal
```css
ul {
    margin: 0;
    padding: 0;
    list-style-type: none;
    width: 720px;
    background: #159cb0 url("../images/fundo-horizontal.png") repeat-x;
    float: left;
}
```

## Layouts em CSS

### Layout Fixo
```css
#container {
    width: 720px;
    margin: 0 auto;
    background: #fff;
}
```

### Layout Líquido
```css
body {
    font-family: Arial, sans-serif;
}

#container {
    width: 90%;
    max-width: 1200px;
    margin: 0 auto;
    background: #fff;
}

#conteudo {
    width: 70%;
    float: left;
}

#sidebar {
    width: 25%;
    float: right;
    background: #d1d1d1;
    padding: 10px;
}

#rodape {
    clear: both;
    background: #c4c4c4;
    padding: 10px;
    text-align: center;
}
```

Esse layout líquido usa porcentagens para adaptar a largura dos elementos ao tamanho da tela, tornando a página mais responsiva.