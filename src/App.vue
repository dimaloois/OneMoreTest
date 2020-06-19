<template>
  <div id="app">
    <div class="wrapper">
      <FirstBlock/>
      <Slider/>
      <Chat/>
    </div>
  </div>
</template>

<script>
import FirstBlock from './components/FirstBlock'
import Slider from './components/Slider'
import Chat from './components/Chat'

export default {
  name: 'App',
  components: {
    FirstBlock,
    Slider,
    Chat,
  }
}
</script>

<style>

@font-face{
	font-family: KievitProBold;
	src: url("./fonts/KievitPro-Bold.ttf");
}
@font-face{
	font-family: KievitProReg;
	src: url("./fonts/KievitPro-Regular.ttf");
}
@font-face{
	font-family: KievitProLight;
	src: url("./fonts/KievitPro-Light.ttf");
}
@font-face{
	font-family: Roboto;
	src: url("./fonts/Roboto-Regular.ttf");
}
/*Обнуление*/
*{
	padding: 0;
	margin: 0;
	border: 0;
}
*,*:before,*:after{
	-moz-box-sizing: border-box;
	-webkit-box-sizing: border-box;
	box-sizing: border-box;
}
:focus,:active{outline: none;}
a:focus,a:active{outline: none;}

nav,footer,header,aside{display: block;}

html,body{
	height: 100%;
	width: 100%;
	font-size: 100%;
	line-height: 1;
	font-size: 14px;
	-ms-text-size-adjust: 100%;
	-moz-text-size-adjust: 100%;
	-webkit-text-size-adjust: 100%;
}
input,button,textarea{font-family:inherit;}

input::-ms-clear{display: none;}
button{cursor: pointer;}
button::-moz-focus-inner {padding:0;border:0;}
a, a:visited{text-decoration: none;}
a:hover{text-decoration: none;}
ul li{list-style: none;}
img{vertical-align: top;}

h1,h2,h3,h4,h5,h6{font-size:inherit;font-weight: 400;}
/*--------------------*/
#app {
  
  background: #F9F7F2;
 
}
.wrapper{
  display: flex;
  min-width: 100%;
  justify-content: center;
  flex-direction: column;
  align-items: center;
}
</style>
