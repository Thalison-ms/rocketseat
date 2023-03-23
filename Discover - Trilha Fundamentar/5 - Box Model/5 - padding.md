# Padding

Preenchimento interno da caixa

- padding-top | padding-right | padding-bottom | padding-left
- values: `<length>` | `<percentage>` | auto

```css
div{
    /*shorthand*/
    margin: 12px 16px 10px 4px;             /*top, right, bottom, left*/
    margin: 12px 16px 0;                    /*top, (right/left), bottom*/
    margin: 8px 16px;           s            /*(top/bottom), (right/left)*/
    margin: 8px;                            /*todos os lados*/
}
```

* Padding poderá causar diferença na largura de um elemento