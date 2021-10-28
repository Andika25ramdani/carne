<template>
	<section class="best-menu text-green py-16">
		<transition name="slide-up" appear>
			<h2 v-if="contentActive" class="font-black text-center title-text pb-12">Our Best Menu</h2>
		</transition>
		<div class="flex flex-1 flex-col sm:flex-row justify-evenly gap-y-8 sm:gap-y-16 mx-auto">
			<figure v-for="menu in menus" :key=menu.id class="menu-figure w-7/12 sm:w-5/12 mx-auto sm:mx-0">
				<div class="menu-image">
					<img :src=menu.img :alt=menu.name class="">
				</div>
				<h2 class="font-black subtitle-text sm:mt-4">{{ menu.name }}</h2>
				<h4 class="font-normal text-default mb-4">{{ menu.subtitle }}</h4>
				<p class="font-normal text-small">{{ menu.desc }}</p>
			</figure>
		</div>
	</section>
</template>

<script>
export default {
	name: 'BestMenu',
	data(){
		return {
			contentActive: false,
			menus: [
				{
					id: 1,
					img: "/img/menus/brisket.png",
					imgAlt: "Brisket",
					name: "Brisket",
					subtitle: "US, AUS, Wagyu",
					desc: "Daging brisket terletak di bagian dada bawah sekitar ketiak sapi. Daging ini juga memiliki keunggulan yaitu teksturnya yang lembut karena banyak lemak."
				},
				{
					id: 2,
					img: "/img/menus/smokedchicken.png",
					imgAlt: "Nasi Briyani Smoked Chicken",
					name: "Smoked Chicken",
					subtitle: "",
					desc: "Daging ayam fillet dengan potongan paha dan dada yang di asap selama 4 jam"
				},
			]
		}
	},
	mounted(){
		this.contentActive = true
	}
}
</script>

<style lang="sass">
.best-menu
	background: url('/img/backgrounds/9.png') no-repeat center center scroll
	background-color: rgba(255, 255, 255, .8)
	background-blend-mode: lighten
.menu-figure
	max-width: 550px
	position: relative
	transition: all .25s ease
	&:hover
		transform: scale(1.0625)
.menu-image
	aspect-ratio: 1.25
	border: 5px solid #003233
	background-color: transparent
	border-radius: 25% / 25%
	transform: scale(.875)
	img
		margin: -5% 0 0 -5%
		border-radius: 25% / 25%
		position: absolute
		transform: scale(1.0625)
</style>