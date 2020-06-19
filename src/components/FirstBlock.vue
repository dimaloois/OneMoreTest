<template>
  <div class = "FirstBlock">
    <div class="FirstBlock__img"> <img src="../imgs/Barselona_isp.png" alt="" class="img1"> </div>
    <div class="FirstBlock__textbox"> 
      <span class="textbox__title"> Барселона — обзор города </span>
      <span class="textbox__text"> Барселона с её золотистыми пляжами, архитектурными шедеврами Гауди, многочисленными фестивалями и гастрономическим разнообразием понравилась мне в первый же день пребывания и стала местом, в котором... </span>
      <a href=""> Читать дальше <span class="textbox__link"></span> </a> 
    </div>
  </div>
</template>

<script>
export default {
  name: 'FirstBlock',
  components: {},
  props: {},
  data() {
    return {}
  },
  mounted() {},
  beforeDestroy() {},
  methods: {}
}
</script>

<style lang="scss" >

  
  
	.FirstBlock {
  display: flex;
  align-content: center;
  align-items: center;
  max-width: 880px;
  width: 100%;
  background: white;
  color: black;
  margin: 110px 20px 0px 20px;
		// .FirstBlock__img

		&__img {
      display: flex;
      background: black;
		}

		// .FirstBlock__text

		&__textbox {
      display: flex;
      max-width: 411px;
      max-height: 440px;
      margin-left: 29px;
      flex-direction: column;
		}

    &__textbox a{
      font-family: KievitProReg;
      color: black;
      font-size: 17px;
      line-height: 25px;
    }
    
    .img1{
      max-width: 440px;
      max-height: 440px;
    }
}

.textbox {

		// .textbox__title

		&__title {
      font-family: KievitProBold;
      font-size: 29px;
      line-height: 35px;
      
		}

		// .textbox__text

		&__text {
      font-family: KievitProLight;
      max-width: 363px;
      font-size: 17px;
      line-height: 25px;
      margin: 19px 0px 7px 0px;
		}

		// .textbox__link

		&__link::before {
    content: '';
    display: block;
    width: 111px;
    height: 3px;
    background: #FF4641;
		}
}



</style>
