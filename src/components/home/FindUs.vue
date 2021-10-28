<template>
  <section class="find-us text-white pb-16">
		<transition name="slide-up" appear>
			<h2 v-if="findTitle" class="font-black text-center title-text pt-8 pb-16">Where To Find Us?</h2>
		</transition>
		<div v-if="contentActive" class="flex flex-1 flex-col sm:flex-row justify-evenly gap-y-16 mx-auto">
			<transition-group name="fade" appear>
				<figure v-for="location in locations" :key=location.id class="loc-figure w-7/12 sm:w-5/12 mx-auto sm:mx-0">
					<div class="loc-image">
						<img :src=location.img :alt=location.imgAlt class="my-8">
						<div class="loc-desc">
							<h2 class="font-black title-text pb-4">{{ location.city }}</h2>
							<h4 class="font-normal subtitle-text">{{ location.address }} <br> {{ location.daysOpen }} <br>{{ location.hoursOpen }}</h4>
						</div>
					</div>
				</figure>
			</transition-group>
		</div>
  </section>
</template>

<script>
export default {
	name: 'FindUs',
	data() {
		return {
			findTitle: false,
			contentActive: false,
			locations: [
				{
					id: 1,
					img: '/img/backgrounds/4.png',
					imgAlt: 'Jalan Aceh',
					city: 'Bandung',
					address: 'Jl. Aceh No. 45',
					daysOpen: 'Mon - Sun',
					hoursOpen: '11.00 - 20.00'
				},
				{
					id: 2,
					img: '/img/backgrounds/5.png',
					imgAlt: 'Jalan Karasak',
					city: 'Bandung',
					address: 'Jl. Karasak No. 109',
					daysOpen: 'Mon - Sun',
					hoursOpen: '11.00 - 20.00'
				},
			]
		}
	},
	mounted () {
		this.findTitle = true
		this.contentActive = true
	}
}
</script>

<style lang="sass">
.find-us
	background: url('/img/backgrounds/3.png') no-repeat center center scroll
	background-color: rgba(0, 50, 51, .9)
	background-blend-mode: hard-light
.loc-figure
	max-width: 683px
	position: relative
	transition: .25s ease
	&:hover
		transform: translate(0, -5%)
.loc-image
	aspect-ratio: 1
	border: 4px solid white
	background-color: transparent
	border-radius: 25% / 25%
	transform: scale(.875)
  position: relative
	img
		margin: -6.25% 0 0 -6.25%
		border-radius: 25% / 25%
		position: absolute
		transform: scale(1.0625)
.loc-desc
  margin: -6.25% 18.75% auto
  position: absolute
  display: flex
  flex-direction: column
  justify-content: center
  height: 100%
</style>