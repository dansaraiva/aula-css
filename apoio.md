# Introdução ao CSS

## O que é CSS?
CSS (Cascading Style Sheets) é uma linguagem de estilização utilizada para definir a apresentação de páginas web. Com o CSS, é possível controlar cores, espaçamentos, fontes, layouts e outros aspectos visuais dos elementos HTML.

## Como o CSS funciona?
O CSS funciona aplicando regras de estilo aos elementos HTML. Essas regras são compostas por seletores e declarações de estilo. Exemplo:
```css
p {
  color: blue;
  font-size: 16px;
}
```
Neste exemplo, todos os parágrafos (`<p>`) serão estilizados com a cor azul e o tamanho de fonte 16px.

## Formas de incluir CSS em um site
Existem três formas principais de incluir CSS em um documento HTML:

1. **CSS Inline**: Estilos aplicados diretamente dentro de um elemento HTML usando o atributo `style`.
   ```html
   <p style="color: red; font-size: 20px;">Texto vermelho</p>
   ```
2. **CSS Interno**: Definição de estilos dentro da tag `<style>` no cabeçalho do HTML.
   ```html
   <style>
     h1 {
       color: green;
     }
   </style>
   ```
3. **CSS Externo**: Utiliza um arquivo separado (`.css`) referenciado no HTML.
   ```html
   <link rel="stylesheet" href="styles.css">
   ```
   **Arquivo styles.css:**
   ```css
   body {
     background-color: lightgray;
   }
   ```

## Seletores CSS
Os seletores definem quais elementos serão estilizados. Alguns exemplos comuns:
- **Seletor de elemento:** `h1 { color: blue; }`
- **Seletor de classe:** `.destaque { font-weight: bold; }`
- **Seletor de ID:** `#menu { background-color: black; }`
- **Seletor de agrupamento:** `h1, h2, p { margin: 10px; }`
- **Seletor descendente:** `div p { color: red; }`

## Trabalhando com Fontes
O CSS permite alterar fontes e tipografias.
```css
p {
  font-family: Arial, sans-serif;
  font-size: 14px;
  font-weight: bold;
  font-style: italic;
}
```
### Explicação das propriedades de fonte:
- **font-family**: Define a família da fonte. Pode ser uma fonte específica ou uma genérica (serif, sans-serif, monospace, etc.).
- **font-size**: Determina o tamanho da fonte (em px, em, %, etc.).
- **font-weight**: Controla a espessura da fonte (normal, bold, lighter, etc.).
- **font-style**: Define o estilo da fonte (normal, italic, oblique).

## Trabalhando com Textos
O CSS também permite manipular a aparência do texto.
```css
p {
  text-align: center;
  text-transform: uppercase;
  text-decoration: underline;
  letter-spacing: 2px;
  line-height: 1.5;
  font-variant: small-caps;
}
```
- **text-align**: Alinha o texto (left, center, right, justify).
- **text-transform**: Transforma o texto (uppercase, lowercase, capitalize).
- **text-decoration**: Adiciona decorações (underline, overline, line-through, none).
- **letter-spacing**: Ajusta o espaçamento entre letras.
- **line-height**: Define a altura da linha do texto.
- **font-variant**: Controla variantes tipográficas, como `small-caps` (exibe letras minúsculas em formato de maiúsculas menores).

## Trabalhando com Cores
O CSS suporta diferentes formatos de cores:
- **Nomes de cores:** `color: red;`
- **Hexadecimal:** `color: #ff0000;`
- **RGB:** `color: rgb(255, 0, 0);`
- **RGBA (transparência):** `color: rgba(255, 0, 0, 0.5);`
- **HSL:** `color: hsl(0, 100%, 50%);`

## Trabalhando com Background
A propriedade `background` permite definir a aparência do fundo dos elementos.
```css
body {
  background-color: lightblue;
  background-image: url('imagem.jpg');
  background-repeat: no-repeat;
  background-position: center;
  background-size: cover;
}
```
### Explicação das propriedades de background:
- **background-color**: Define a cor de fundo.
- **background-image**: Define uma imagem de fundo.
- **background-repeat**: Controla a repetição da imagem (repeat, no-repeat, repeat-x, repeat-y).
- **background-position**: Define a posição da imagem (center, top left, bottom right, etc.).
- **background-size**: Define o tamanho da imagem de fundo (cover, contain, auto, valores específicos).

## Conclusão
O CSS é uma ferramenta essencial para o design de sites, permitindo criar interfaces atraentes e responsivas. Dominar seletores, fontes, cores e formas de aplicação ajudará a estilizar qualquer página web de maneira eficiente!