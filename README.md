#Monday
## Flexbox
Flexbox always target the parent container
### flex-direction: row/column
Display items horizontally/ vertically
### justify-content: center, space-around, space-between: 
Use the same direction as **flex-direction**. If **flex-direction** is vertical, **justify-content** adjust vertical and vice versa
### align-items: center/ flex-end/ flex-start
Use the opposit direction of flex-direction. If **flex-direction** is vertical, **align-item** is vertical and vice versa
~~~
#parent {
display: flex;
flex-direction: column
justify-content: space-around;
align-items: center;
}
~~~
#Tuesday
## Emnet syntax
create multiple tag with class in mass, id without typing manually
~~~
div.square*5 enter -> create 5 div with class square
div.container>div#item${ITEM $}*5 -> create 1 div container that has 5 children div with id = item1 - item5 and has the text range from 'ITEM 1' to 'ITEM 5'
~~~
create number from a certain number: $@17
~~~
div.container>div.square{$@17}*10
        <div class="container">
            <div class="square">17</div>
            <div class="square">18</div>
            <div class="square">19</div>
            <div class="square">20</div>
            <div class="square">21</div>
        </div>
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
#Wednesday
## grid
To layout whole website (flex can be applied to smaller section like nav, header, etc)
~~~
.app{
display: grid;
grid-template-columns: 1fr 2fr 1fr;
grid-template-rows: 1fr 2fr 1fr;
grid-template-areas:
"img1 img1 img2"
"img1 img1 img2"
;
}
.img1 {
grid-row: 1/2; // or 1 span 1
grid-column: 1/2; // or 1 span 2
// if use grid area, don't need grid-row or grid-column
grid-area: img1;
}
.img2 {
grid-row: 2/2; // or 2 span 1
grid-column: 2/1; // or 2 span 1
// or use grid area
grid-area: img2;
}
~~~
#Thursday
## Arrow function
this
~~~
const add = (a,b) => a+b
const add = (a,b) => {return a+b} //-> need {} if there are more complicated things inside
const timeFive = (a) => a * 5 //-> prefered
const timeFive = a => a * 5
~~~
equal this expressive function:
~~~
const add = function (a,b) {
  return a+b
}
~~~
Ex: </br>
profestion way:
~~~
const names = (todos) => todos.map((todo) => todo.text)
~~~
Also can do this: (not as clear)
~~~
const names2 = todos => todos.map(todo => todo.text)
~~~
if take 1 parameter, don't need ()
~~~
const add = (n) => n + 5;
~~~
equal this (doesn't look like function but works)
~~~
const add3 = n => n + 5;
~~~
