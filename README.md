#Javascript Crash Course - Magic 8Ball
###Context: HTML | CSS | Javascript
[Examples of the demo with HTML , HTML + CSS,  HTML + CSS + JavaScript](http://t3patterson.github.io/crashcourse-html-css-js-scratch-padl/)

###The Crash Course:  on Codepen 
[Starting Point](http://codepen.io/tphdevdrop/pen/zBWrWG)
[Complete Demo](http://codepen.io/tphdevdrop/pen/zBWkAk)  

###Explanation of Walkthrough (in codepen)
#####HTML

note: in codepen `div*398` + *tab* key will give you 398 div tags for the necessary 400 divs

```html
<h1>Scratch Pad</h1>

<main id="canvas">
  <div></div> 
  <div class="show-selected"></div>
  <!--div*398-->
</main>
```

#####CSS
```css
*{
  box-sizing: border-box;
}

h1{
  font-family: 'Helvetica';
  font-weight: 200;
  border-bottom: 2px solid #67809F;
}

main {
  /*background: lightgreen ... for demo of size*/
  display: flex;
  flex-flow: row wrap;
  width: 400px;
  margin: 0 auto;
}

div{
  width: 20px;
  height: 20px;
  border: 1px solid #999;
}

div.show-selected{
  background: navy;
  opacity: 1;
}
```


#####JS
```
function showSelected(input){
  var htmlEl = input.target
  $(htmlEl).addClass('show-selected')
}

$('div').on('click', showSelected)
```