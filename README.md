#Monday
## Flexbox
Flexbox always target the parent container
~~~
#parent {
display: flex;
justify-content: space-around;
align-item: center;
}


~~~
#Tuesday
## Emnet syntax
create multiple tag with class in mass, id without typing manually
~~~
div.square*5 enter -> create 5 div with class square
div.container>div#item${ITEM $}*5 -> create 1 div container that has 5 children div with id = item1 - item5 and has the text range from 'ITEM 1' to 'ITEM 5'
~~~
## @media
Responsive width of screen:
If css default is dekstop -> tablet -> mobile
~~~
@media (max-width: 800px) {} //-> width < 800px
@media (max-width: 400px) {} //-> width < 400px
~~~
or
~~~
@media (max-width: 800) and (min-width: 401px) {} 401 <= width < 800
~~~
if css default is mobile -> tablet -> desktop (Preferway)
~~~
@media (min-width: 400px) {}  //-> 400px < width
@media (min-width: 800px) {}  //-> 800px < width
~~~
or
~~~
@media (min-width: 401px) and (max-width: 801px) {} 400px < width <= 799px
~~~
