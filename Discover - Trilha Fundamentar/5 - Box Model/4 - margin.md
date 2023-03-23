## Margin

Espaços entre os elementos

- margin-top | margin-right | margin-bottom | margin-left
- values: `<length>` | `<percentage>` | auto

```css
div{
    /*shorthand*/
    margin: 12px 16px 10px 4px;             /*top, right, bottom, left*/
    margin: 12px 16px 0;                    /*top, (right/left), bottom*/
    margin: 8px 16px;                       /*(top/bottom), (right/left)*/
    margin: 8px;                            /*todos os lados*/
}
```

* Cuidado com margin collapsing (top se ajunda ao bottom) 