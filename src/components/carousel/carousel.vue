<template>
	<div class="carousel">
		<slot></slot>
		<!-- <img class="carousel__nav caroussel__prev p-a1" src="../../img/fleche.svg" @click.prevent="prev"  :class="colorArrow()" alt=""> -->
		<arrowLeft class="carousel__nav caroussel__prev p-a1" @click.prevent="next" :class="colorArrow()"/>
		<arrowRight class="carousel__nav caroussel__next p-a2" @click.prevent="next" :class="colorArrow()"/>
			
		
	<footer>
      <div class="d-flex1">
        <div>
          <ul class="reseau">
            <li><a href="#"><i class="demo-icon icon-mail-alt"></i></a></li>
            <li><a href="https://www.linkedin.com/in/quentin-rulleau-4b5822179/"><i class="demo-icon icon-linkedin"></i></a></li>
            <li><a href="https://www.instagram.com/lepetitdevweb/"><i class="demo-icon icon-instagram"></i></a></li>
            <li class="language"><a href="#">EN</a></li>
          </ul>
        </div>
        <div>
          <ul class="cercle">
            <li></li>
            <li></li>
            <li></li>
            <li></li>
          </ul>
        </div>
        <p class="copyright">Quentin Rulleau ®. All rights reserved.</p>
      </div>
    </footer>		
	</div>
</template>
<script>
	import arrowLeft from '../../assets/arrowLeft.vue'
	import arrowRight from '../../assets/arrowRight.vue'


	export default {
		components: {
			arrowLeft,
			arrowRight
			
		},
		data () {
			return {
				index: 0,
				slides: this.$children,
				direction: 'right'
			}
		},
		mounted () {
			this.slides = this.$children
			this.slides.forEach ((slide, i) => {
				slide.index = i
			})
		},
		computed: {
			transition () {
				return 'slide-' + this.$parent.direction
			},
			slidesCount () {
				return this.slides.length
			}
		},
		methods: {
			next () {
				this.index++
				this.direction = 'right'
				if (this.index >= this.slidesCount){
					this.index = 0
				}
			},
			prev () {
				this.index--
				this.direction = 'left'
				if (this.index < 0){
					this.index = this.slidesCount - 1
				}
			},
			colorArrow () {
				if (this.index === 1){
					return 'blanc'
				}
				if (this.index === 2){
					return 'orange'
				}
				if (this.index === 3 ){
					return 'orange'
				}
			}
			
		}
	}
</script>

<style>
.blanc {
	fill: #ffffff;
}
</style>