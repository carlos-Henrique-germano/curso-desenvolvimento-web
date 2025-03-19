# Guia Didático de Seletores e Layouts CSS

Este guia apresenta diversos seletores e conceitos de CSS comentados, com explicações sobre seu funcionamento.

## Seletores CSS

### 1. \*\*Seletor Universal (`*`)

\*\*
O seletor universal aplica um estilo a todos os elementos da página.

```css
* {
    border: 1px solid red;
}
```

---

### 2. **Seletor de Texto**

O seletor de texto estiliza elementos HTML pelo nome da tag.

```css
h1 {
    color: green;
}
```

---

### 3. **Seletor de Classe**

Define um estilo para todos os elementos que possuem a classe especificada.

```css
.brown {
    color: brown;
}

p.brown {
    color: brown;
}
```

---

### 4. **Seletor de ID**

Define um estilo específico para um elemento identificado por um `id`.

```css
#header {
    border: 1px solid blue;
}
```

---

### 5. **Seletor de Filho (****`>`****)**

Aplica estilos apenas aos elementos que são filhos diretos de outro.

```css
li > a {
    color: red;
    text-decoration: none;
}
```

---

### 6. **Seletor de Descendente (espaço)**

Afeta qualquer elemento dentro de outro, independentemente da hierarquia direta.

```css
p a {
    color: green;
}
```

---

### 7. **Seletor de Irmão Adjacente (****`+`****)**

Aplica estilo ao primeiro elemento que aparece logo após outro elemento.

```css
h1 + p {
    color: darkorange;
    font-size: 32px;
}
```

---

### 8. **Seletor de Irmão Geral (****`~`****)**

Seleciona todos os elementos que são "irmãos" do elemento anterior.

```css
h3 ~ p {
    color: hotpink;
    font-size: 24px;
}
```

---

## Herança e Especificidade CSS

Quando regras se sobrepõem, a mais específica tem precedência.

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
```

---

## Barra de Navegação Vertical

```css
ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
}

ul a {
    width: 200px;
    height: 40px;
    display: block;
    color: #000;
    background: #f7b600 url("../images/menu.png") no-repeat left bottom;
    text-decoration: none;
    text-indent: 30px;
    line-height: 40px;
}
```

---

## Barra de Navegação Horizontal

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

---

## Layouts e Estruturação CSS

```css
#container {
    width: 720px;
    margin: 0 auto;
    background: #fff;
}

#conteudo {
    width: 520px;
    float: right;
}

#navegacao {
    width: 180px;
    float: left;
    background: #d1d1d1;
}

#rodape {
    clear: both;
    background: #c4c4c4;
    padding: 5px;
    text-align: center;
}
```

