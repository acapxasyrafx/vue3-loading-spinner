<template>
  <div id="app">
    <div class="header">
      <h1 class="header--title">vue-loading-spinner v1.0</h1>
    </div>
    <div class="intro">
      <p>Just another collection of loading spinners with Vue.js, a lot of spinners</p>
      <a class="btn" href="https://github.com/nguyenvanduocit/vue-loading-spinner">Github</a>
    </div>
    <div class="spinner-list">
      <div class="spinner-container" v-for="spinner in spinners" :key="spinner.path">
        <component :is="spinner.component" :size="size"></component>
        <div class="name">{{ spinner.path }}</div>
      </div>
    </div>
  </div>
</template>

<script>
import RotateSquare from './components/RotateSquareShape'
import RotateSquare2 from './components/RotateSquare2Shape'
import RotateSquare3 from './components/RotateSquare3Shape'
import RotateSquare4 from './components/RotateSquare4Shape'
import RotateSquare5 from './components/RotateSquare5Shape'
import RotateSquare6 from './components/RotateSquare6Shape'
import DoubleBounce from './components/DoubleBounceShape'
import Stretch from './components/StretchShape'
import CubeShadow from './components/CubeShadowShape'
import ScaleOut from './components/ScaleOutShape'
import CircleSpin from './components/CircleShape'
import CircleSpin2 from './components/Circle2Shape'
import CircleSpin3 from './components/Circle3Shape'
import CircleSpin4 from './components/Circle4Shape'
import CircleSpin5 from './components/Circle5Shape'
import CircleSpin6 from './components/Circle6Shape'
import CircleSpin7 from './components/Circle7Shape'
import CircleSpin8 from './components/Circle8Shape'
import CircleSpin9 from './components/Circle9Shape'
import CircleSpin10 from './components/Circle10Shape'
import CircleSpin11 from './components/Circle11Shape'
import ThreeDots from './components/ThreeDotsShape'
import GoogleSpin from './components/GoogleShape'
import Gauge from './components/GaugeShape'
import Origami from './components/OrigamiShape'
import Hexagon from './components/HexagonShape'
import Socket from './components/SocketShape'
import HourGlass from './components/HourGlassShape'
import Pencil from './components/PencilShape'
import Jawn from './components/JawnShape'
import LetterCube from './components/LetterCubeShape'
import PingPong from './components/PingPongShape'
import Diamond from './components/DiamondShape'
import SpinLine from './components/SpinLineShape'
import Plane from './components/PlaneShape'
import Mikepad from './components/MikepadShape'
import Jumper from './components/JumperShape'
import Wave from './components/WaveShape'
import Texture from './components/TextureShape'

export default {
  name: 'App',
  components: {
    RotateSquare,
    RotateSquare2,
    RotateSquare3,
    RotateSquare4,
    RotateSquare5,
    RotateSquare6,
    DoubleBounce,
    Stretch,
    CubeShadow,
    ScaleOut,
    CircleSpin,
    CircleSpin2,
    CircleSpin3,
    CircleSpin4,
    CircleSpin5,
    CircleSpin6,
    CircleSpin7,
    CircleSpin8,
    CircleSpin9,
    CircleSpin10,
    CircleSpin11,
    ThreeDots,
    GoogleSpin,
    Gauge,
    Hexagon,
    Socket,
    Origami,
    HourGlass,
    Pencil,
    Jawn,
    LetterCube,
    PingPong,
    Diamond,
    SpinLine,
    Plane,
    Mikepad,
    Jumper,
    Wave,
    Texture
  },
  data() {
    return {
      spinners: [
      { path: 'RotateSquare', component: 'RotateSquare' },
        { path: 'RotateSquare2', component: 'RotateSquare2' },
        { path: 'RotateSquare3', component: 'RotateSquare3' },
        { path: 'RotateSquare4', component: 'RotateSquare4' },
        { path: 'RotateSquare5', component: 'RotateSquare5' },
        { path: 'RotateSquare6', component: 'RotateSquare6' },
        { path: 'DoubleBounce', component: 'DoubleBounce' },
        { path: 'Stretch', component: 'Stretch' },
        { path: 'CubeShadow', component: 'CubeShadow' },
        { path: 'ScaleOut', component: 'ScaleOut' },
        { path: 'CircleSpin', component: 'CircleSpin' },
        { path: 'CircleSpin2', component: 'CircleSpin2' },
        { path: 'CircleSpin3', component: 'CircleSpin3' },
        { path: 'CircleSpin4', component: 'CircleSpin4' },
        { path: 'CircleSpin5', component: 'CircleSpin5' },
        { path: 'CircleSpin6', component: 'CircleSpin6' },
        { path: 'CircleSpin7', component: 'CircleSpin7' },
        { path: 'CircleSpin8', component: 'CircleSpin8' },
        { path: 'CircleSpin9', component: 'CircleSpin9' },
        { path: 'CircleSpin10', component: 'CircleSpin10' },
        { path: 'CircleSpin11', component: 'CircleSpin11' },
        { path: 'ThreeDots', component: 'ThreeDots' },
        { path: 'GoogleSpin', component: 'GoogleSpin' },
        { path: 'Gauge', component: 'Gauge' },
        { path: 'Hexagon', component: 'Hexagon' },
        { path: 'Socket', component: 'Socket' },
        { path: 'Origami', component: 'Origami' },
        { path: 'HourGlass', component: 'HourGlass' },
        { path: 'Pencil', component: 'Pencil' },
        { path: 'Jawn', component: 'Jawn' },
        { path: 'LetterCube', component: 'LetterCube' },
        { path: 'PingPong', component: 'PingPong' },
        { path: 'Diamond', component: 'Diamond' },
        { path: 'SpinLine', component: 'SpinLine' },
        { path: 'Plane', component: 'Plane' },
        { path: 'Mikepad', component: 'Mikepad' },
        { path: 'Jumper', component: 'Jumper' },
        { path: 'Wave', component: 'Wave' },
        { path: 'Texture', component: 'Texture' },
      ],
      size: '60px', // Default size for the spinners
    };
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.header {
  margin-bottom: 20px;
}

.header--title {
  font-size: 2em;
  margin-bottom: 10px;
}

.intro {
  margin-bottom: 40px;
}

.btn {
  margin-top: 20px;
  padding: 10px 30px;
  border-radius: 30px;
  display: inline-block;
  color: #fff;
  background-color: #4fc08d;
  transition: all 0.15s ease;
  box-sizing: border-box;
  text-transform: uppercase;
  text-decoration: none;
  &:hover{
    background-color: #57d69c;
  }
}

.btn:hover {
  background-color: #42b983;
  color: white;
}

.spinner-list{
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: row;
  flex-wrap: wrap;
}
.spinner-container{
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  min-height: 250px;
  min-width: 250px;
  width: 25%;
  overflow: hidden;
  .name{
    margin-top: 10px;
    color: #41b883;
    font-size: 16px;
  }
}
</style>