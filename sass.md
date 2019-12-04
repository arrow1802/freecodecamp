<!-- 5 -->
<style type='text/sass'>

@for $j from 1 through 6 {
    .text-#{$j} { font-size : $j*10px}
}

</style>

<p class="text-1">Hello</p>
<p class="text-2">Hello</p>
<p class="text-3">Hello</p>
<p class="text-4">Hello</p>
<p class="text-5">Hello</p>


<!-- 6 -->
<style type='text/sass'>

@each $color in blue, black, red {
  .#{$color}-bg {background-color: $color;}
}


  div {
    height: 200px;
    width: 200px;
  }
</style>

<div class="blue-bg"></div>
<div class="black-bg"></div>
<div class="red-bg"></div>



<!-- 7 -->

<style type='text/sass'>
$x:1;
@while $x < 6 {
    .text-#{$x} { font-size : $x*15px;} 
    $x: $x + 1;
}


</style>

<p class="text-1">Hello</p>
<p class="text-2">Hello</p>
<p class="text-3">Hello</p>
<p class="text-4">Hello</p>
<p class="text-5">Hello</p>

<!-- 8 -->

// The main.scss file
@import "variables"

<!-- 9 -->

<style type='text/sass'>
  h3{
    text-align: center;
  }
  .info{
    width: 200px;
    border: 1px solid black;
    margin: 0 auto;
  }
  .info-important {
    @extend .info;
    background-color : magenta;
  }




</style>
<h3>Posts</h3>
<div class="info-important">
  <p>This is an important post. It should extend the class ".info" and have its own CSS styles.</p>
</div>

<div class="info">
  <p>This is a simple post. It has basic styling and can be extended for other uses.</p>
</div>
