<template>
  <div id="app">
    <!--<canvas id="canvas">-->
    <!--<canvas id="demo-canvas"></canvas>-->
      <router-view></router-view>
    </canvas>
  </div>
</template>

<script>
  export default {
    name: 'app'
  }
  // jQuery(document).ready(function ($) {
  //   let windowXArray = []
  //   let windowYArray = []
  //   for (let i = 0; i < $(window).innerWidth(); i++) {
  //     windowXArray.push(i)
  //   }
  //   for (let i = 0; i < $(window).innerHeight(); i++) {
  //     windowYArray.push(i)
  //   }
  //   function randomPlacement (array) {
  //     var placement = array[Math.floor(Math.random() * array.length)]
  //     return placement
  //   }
  //   var canvas = oCanvas.create({
  //     canvas: '#canvas',
  //     background: '#2c3e50',
  //     fps: 60
  //   })
  //   setInterval(function () {
  //     var rectangle = canvas.display.ellipse({
  //       x: randomPlacement(windowXArray),
  //       y: randomPlacement(windowYArray),
  //       origin: { x: 'center', y: 'center' },
  //       radius: 0,
  //       fill: '#27ae60',
  //       opacity: 1
  //     })
  //     canvas.addChild(rectangle)
  //     rectangle.animate(
  //       {
  //         radius: 10,
  //         opacity: 0
  //       },
  //       {
  //         duration: '1000',
  //         easing: 'linear',
  //         callback: function () {
  //           this.remove()
  //         }
  //       }
  //     )
  //   }, 100)

  //   $(window).resize(function () {
  //     canvas.width = $(window).innerWidth()
  //     canvas.height = $(window).innerHeight()
  //   })
  //   $(window).resize()
  // })
</script>

<style>
  @import './assets/css/hexagons.css';

  body {
    background: #15191e;
    /*background: white
    background: #00CAF9
    background: #0ba9f0*/
    margin: 0;
  }
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
  }

  #canvas {
    width: 100%;
    height: 100%;
  }
</style>
