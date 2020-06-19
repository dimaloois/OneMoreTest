<template>
    <div class="Slider">
      <div class="Slider__title">Отзывы о Барселоне</div>
      <slick
  ref="slick"
  :options="slickOptions"
  >     
        <div class="Slider__item"
                  v-for="(i, index) in itemsCounter"
                  :key="index">
          <div class="item__header"> <img src="../imgs/avatar.png" alt=""> <span>Наталия Полянская</span>  </div>
          <div class="item__title"> <span>Барселона</span> - о городе: </div>
          <div class="item__text"> Барселона – моя третья большая любовь, после Вены и Крита. Это город, в который я каждый раз возвращаюсь с огромным <br> удовольствием, всем <br>
рекомендую хоть раз там <br>
побывать и осмотреть ... </div>
          <div class="item__imgs"> <img src="../imgs/comment_1.png" alt=""> <img src="../imgs/comment_2.png" alt=""> <img src="../imgs/comment_3.png" alt=""> <img src="../imgs/comment_3.png" alt=""> </div>
          <div class="item__footer"> <span>около 1 года назад</span> . <span>9 комментариев</span> <img src="../imgs/like.png" alt=""> 7 </div>
        </div>
  
</slick>
<button class="allComentsButton">Все отзывы</button>
    </div>
</template>

<script>
import Slick from 'vue-slick';

export default {
  name: 'Slider',
  components: {
    Slick
  },
  props: {},
  data() {
    return {
      itemsCounter:18,
       slickOptions: {
              slidesToShow: 3,
              slidesToScroll: 3,
              dots: true,
              arrows: false,
              variableWidth: true,
            },
            images:[
              '../imgs/comment_1.png',
              '../imgs/comment_1.png',
              '../imgs/comment_1.png',
            ],
            index:null,
    }
  },
  mounted() {
  },
  beforeDestroy() {},
  methods: {}
}
</script>

<style lang="scss">



.Slider {
  display: flex;
  margin-top: 20px;
  background: white;
  padding: 35px 31px 49px 31px;
  flex-direction: column;
  max-width: 880px;
		// .Slider__item

		&__item {
      background: #F9F7F2;
      max-width: 300px;
      margin: 0px 20px;
      font-family: KievitProReg;
      font-weight: 500;
    }
    &__title{
      display: flex;
      font-family: KievitProBold;
      margin: 35px 0 21px 0;
      font-size: 29px;
      line-height: 35px;
      letter-spacing: 0.03em;
      max-width: 300px;
      width: 100%;
      margin-left: 20px;
    }
}
.item {

		// .item__header

		&__header {
      display: flex;
      align-items: center;
      margin: 26px 0 0 19px;
    }
    &__header span{
      margin-left: 10px;
      font-size: 15px;
      line-height: 17px;
    }

		// .item__title

		&__title {
      margin: 28px 0px 12px 0px;
      margin: 26px 0 0 19px;
    }
    &__title span{
      font-family: KievitProReg;
      font-weight: 600;
      color: #FC4F1E;
      font-size: 13px;
      line-height: 17px;
      letter-spacing: 0.464286px;
      text-transform: uppercase;
      
    }

		// .item__text

		&__text {
      font-size: 15px;
      font-family: Roboto;
      line-height: 25px;
      max-width: 272px;
      margin: 26px 0 0 19px;
		}

		// .item__imgs

		&__imgs {
      margin: 26px 0 0 19px;
    }
    &__imgs img{
    margin: 8px 2.5px 26px 2.5px;
    }
		// .item__footer

		&__footer {
      font-size: 11px;
      margin: 0 0 11px 19px;
    }
    &__footer img{
      margin-left: 50px;
    }
}

.allComentsButton{
  display: flex;
  height: 40px;
  max-width: 124px;
  justify-content: center;
  align-items: center;
  font-size: 15px;
  font-family: KievitProReg;
  font-weight: 600;
  position: relative;
  margin-left: 23px;
  border: 2px solid #FF4641;
  background: white;
}




 .Slider .slick-slider {
  min-width: 0;
}
.Slider .slick-list {
	overflow: hidden;
}
.Slider .slick-track {
	display: flex;
}
.Slider .slick-dots {
	margin: 32px 0 0 0;
	display: flex;
	align-items: flex-end;
	justify-content: flex-end;
}
 .Slider  .slick-dots li {
	list-style: none;
	margin: 0 10px;
}
.Slider .slick-dots button {
	font-size: 0;
	width: 4px;
	height: 4px;
	background-color: #212121;
	border-radius: 50%;
}
.Slider .slick-dots li.slick-active button{
	background-color: #FF4641;
	width: 8px;
	height: 8px;
	margin: 0 -2px;
}

</style>
