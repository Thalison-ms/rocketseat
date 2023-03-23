# Distâncias absolutas <length>

São fixas e não alteram seu valor.

Unidade          Nome                       Equivalência
cm               Centímestro                1cm = 96px/2.54
in               Inches (polegadas)         1in = 2.54cm = 96px
px               Pixiels                    1px = 1/96th of 1in

* O mais comum e mais utilizado é o **px**
* Não recomendado usar cm

# Distâncias relativas

São relativas a algum outro valor, pode ser o elemento pai, ou root, ou o tamanho da tela.

* Benefício: Maior adaptação aos diferentes tipos de tela

Unidade         Relativo a
em              Tamanho da font do pai
rem             Tamanho da font do elemento raiz (root/html)
vw              1% da viewport width
vh              1% da viewport height

# Exemplos
===========================================================================================
Usando em
```css
div{
    font-size: 18px;
}

p{
    font-size: 2em;
}

```
No exemplo acima podemos ver que a div foi configurada com 18px, ou seja é o bloco pai
Agora caso a tag p esteja dentro da div, 2em significa que irá multiplicar 18px por 2, ficando com 36px
Caso fosse 1em, não iria ocorrer alteração no tamanho 18

===========================================================================================
Usando rem
```css
:root{

}
html{
    font-size: 12px;
}
div{
    font-size: 18px;
}

p{
    font-size: 2rem;
}
```
No caso do rem, por mais que a tag <p> esteja dentro da tag <div>, o CSS irá buscar o elemento raiz que seria a tag <html> ou :root
Supondo que fosse o html, nesse caso <p> seria multiplicado pelo tamanho em <html> que é 12, fazendo assim que <p> seja igual a 24px
===========================================================================================
# IMPORTANTE
Por padrão o html não tem um valor padrão para altura, ou seja, height, então é necessário definir uma altura em algum elemento raiz, seja ele 
:root, html ou body

