<template>
  <section class="available bg-green text-white text-right flex flex-col sm:flex-row items-center p-8 sm:p-0">
		<img src="/img/backgrounds/8.png" alt="Party" class="mx-auto">
		<div class="flex flex-col w-5/6 sm:w-full sm:py-4 sm:pr-4 md:py-8 md:pr-8 lg:my-12 lg:mr-12 xl:my-16 xl:mr-16">
		<transition-group name="slide-right">
			<h2 v-if="contentActive" class="font-black title-text py-6 sm:pb-12 border-b-4 border-white">Do You Like to Party? Level Up Your Game With Carne To Impress Everyone Bellys</h2>
			<h3 v-if="contentActive" class="font-black subtitle-text py-6 sm:py-12">We Are Available For</h3>
			<div class="flex flex-row flex-nowrap w-full justify-between">
				<ul v-if="contentActive" class="list-none list-outside">
					<li class="subtitle-text font-bold">Collaboration</li>
					<li class="subtitle-text font-light">Coffee Shop</li>
					<li class="subtitle-text font-light">Restaurant</li>
					<li class="subtitle-text font-light">Bar/Lounge</li>
				</ul>
				<ul v-if="contentActive" class="list-none list-outside">
					<li class="subtitle-text font-bold">Private Event</li>
					<li class="subtitle-text font-light">Wedding</li>
					<li class="subtitle-text font-light">Barbecue Night</li>
					<li class="subtitle-text font-light">Private Party</li>
				</ul>
			</div>
		</transition-group>
		</div>
	</section>
</template>

<script>
export default {
  name: 'Available',
  data() {
	  return {
		  contentActive: false
	  }
  },
  mounted() {
	  this.contentActive = true
  }
}
</script>

<style lang="sass">
.available img
	width: 81%
	object-fit: contain
	@media screen and (min-width: 640px)
		width: 51%
</style>