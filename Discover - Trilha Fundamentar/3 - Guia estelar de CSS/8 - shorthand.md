# Shorthand

* Junção de propriedades
* resumido
* legível

```css
{
    /*background properties*/
    background-color: #000;
    background-image: url(images/bg.gif);
    background.repeat: no-repeat;
    background-position: left top;

    /*background shorthand*/
    background: #000 url(images/bg.gif) no-repeat left top;

    /*font properties*/
    font-style: italic;
    font-weight: bold;
    font-size: .8rem;
    line-height: 1.2;
    font-family: Arial, sans-serif;

    /*font shorthand*/
    font: italic bold .8rem/1.2 Arial, sans-serif;
}
```

# Detalhes

* Não irá considerar propriedades anteriores
* Valores não especificados irão assumir o valor padrão
* Geralmente, a ordem descrita não importa, mas, se houver muitas propriedades com valores semelhantes, poderemos encontrar problemas.

## Propriedades que aceitam shorthand

animation
border, border-bottom, border-color, border-left, border-radius, border-right, border-style, border-top, border-width
column-rule, columns
flex, flex-flow
font
grid, grid-area, grid-column, grid-row, grid-template
list-style
margin, margin-top, margin-right, margin-bottom, margin-left
ofsset, outline, overflow
padding, padding-top, padding-right, padding-bottom, padding-left
place-content, place-items, place-self
text-decoration
transition

**https://developer.mozilla.org/en-US/docs/Web/CSS/Shorthand_properties**