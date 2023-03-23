# Porcentagens

* Em muitos casos é tratado da mesma maneira que as distâncias <length>
* Sempre será relativo a algum valor
=================================================
```css
html{
    font-size: 50%
}

```

Quando passamos uma informação de porcentagem direto no HTML e não se tem um elemento pai, raiz/root, ele pega em relação a informação padrão do 
navegador, que seria 16px, então 50% em relação a 16px padrão seria 8px.
=================================================
```html
<ul>
    <li>One</li>
    <li>Two</li>
    <li>Three
        <ul>
            <li> Three A</li>
            <li> Three B
                <ul>
                    <li>Three B 2</li>
                </ul>
            </li>
        </ul>
    </li>
</ul>
```
```css
li{
    font-size: 50%;
}
```
* No exemplo acima, 50% do primeiro li seria em cima dos 16px padrão, logo seria 8px
* No segundo li 50% seria referente ao elemento pai, que seria o primeiro li que vale 8px, logo o segundo li seria 4px
* No terceilo li 50% de 4px seria 2px e assim seria para os próximos li filhos
=================================================
```css
body{
    width: 50%
}
div{
    backgroud-color: blue;
    width:50%
}
```
* No caso acima temos definido que body precisa ter 50% em relação a alguém, como não temos definido nada para html/root, o padrão é a tela.
* Então sabemos que body irá ocupar só metade da tela
* Tendo essa div, configurada em 50% também, ela irá ocupar metade do body
* Então a div irá ocupar 1/4 da tela