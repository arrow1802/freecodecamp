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