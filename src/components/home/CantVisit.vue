<template>
  <section class="cant-visit text-green px-4 sm:px-16 lg:px-32 py-16">
		<h2 class="font-black title-text px-8 sm:px-0">Oh no! You Can’t Visit Us?!</h2>
		<h3 class="subtitle-text py-4 sm:py-0 sm:pb-4 px-8 sm:px-0">No Worry We Got You Covered</h3>
		<div class="visit-section">
			<p class="text-default px-8 sm:px-0">with our partner, now you can have the best of our meats send straight to your house!</p>
			<img src="/img/backgrounds/7.png" alt="Take Away Service" class="contact-figure w-11/12 sm:w-6/12 mx-auto sm:mr-0 sm:ml-auto mt-12 sm:-mt-8">
			<div class="flex flex-col items-center sm:float-left mt-8 sm:-mt-12">
				<a href="" class="flex-none">
					<img src="/img/partners/grabfood.png" alt="Book GrabFood" class="image-link px-4 sm:px-0 sm:pr-16 md:pr-12 lg:pr-8 xl:pr-4">
				</a>
				<a href="" class="flex-none">
					<img src="/img/partners/gofood.png" alt="Book gofood" class="image-link px-4 sm:px-0 sm:pr-16 md:pr-12 lg:pr-8 xl:pr-4">
				</a>
				<!-- <a href="" class="flex-1">
					<img src="" alt="Book GrabFood">
				</a> -->
			</div>
		</div>
	</section>
</template>

<script>
export default {
  name: 'CantVisit'
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