<template>
  <section class="cant-visit text-green px-4 sm:px-16 lg:px-32 py-16">
	  <transition-group name="slide-left">
		<h2 v-if="contentActive" class="font-black title-text px-8 sm:px-0">Oh no! You Can’t Visit Us?!</h2>
		<h3 v-if="contentActive" class="subtitle-text py-4 sm:py-0 sm:pb-4 px-8 sm:px-0">No Worry We Got You Covered</h3>
	  </transition-group>
		<div class="visit-section">
			<transition name="slide-left">
				<p v-if="contentActive" class="text-default px-8 sm:px-0">with our partner, now you can have the best of our meats send straight to your house!</p>
			</transition>
			<transition name="slide-right">
				<img v-if="contentActive" src="/img/backgrounds/7.png" alt="Take Away Service" class="contact-figure w-11/12 sm:w-6/12 mx-auto sm:mr-0 sm:ml-auto mt-12 sm:-mt-8">
			</transition>
			<div class="flex flex-col items-center sm:float-left mt-8 sm:-mt-12">
				<transition-group name="slide-up">
					<a v-if="contentActive" href="" class="flex-none">
						<img src="/img/partners/grabfood.png" alt="Book GrabFood" class="image-link px-4 sm:px-0 sm:pr-16 md:pr-12 lg:pr-8 xl:pr-4">
					</a>
					<a v-if="contentActive" href="" class="flex-none">
						<img src="/img/partners/gofood.png" alt="Book gofood" class="image-link px-4 sm:px-0 sm:pr-16 md:pr-12 lg:pr-8 xl:pr-4">
					</a>
				</transition-group>
			</div>
		</div>
	</section>
</template>

<script>
export default {
  name: 'CantVisit',
  data() {
	  return {
		  contentActive: false
	  }
  },
  mounted(){
	  this.contentActive = true
  }
}
</script>

<style lang="sass">
.cant-visit
	background: url('/img/backgrounds/6.png') no-repeat center center scroll
	background-size: auto
	background-color: rgba(255, 255, 255, .85)
	background-blend-mode: lighten
.visit-section
	p
		max-width: 625px
		@media screen and (min-width: 640px)
			max-width: 55%
	img.image-link
		height: 100%
		max-width: 10rem
</style>