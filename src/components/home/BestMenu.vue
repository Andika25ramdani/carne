<template>
	<section class="best-menu text-green pb-16">
		<h2 class="font-black text-center title-text pt-8 pb-8">Our Best Menu</h2>
		<div class="flex flex-1 flex-col md:flex-row justify-evenly gap-y-16 mx-auto">
			<figure class="menu-figure w-11/12 md:w-5/12 mx-auto md:mx-0">
				<div class="menu-image">
					<img src="/img/peoples/people-2.jpg" alt="Graha Wibisana" class="my-8">
				</div>
				<h2 class="font-black title-text mt-12">Brisket</h2>
				<h4 class="font-normal text-4xl mb-4">US, AUS, Wagyu</h4>
				<p class="font-normal text-2xl">Daging brisket terletak di bagian dada bawah sekitar ketiak sapi. Daging ini juga memiliki keunggulan yaitu teksturnya yang lembut karena banyak lemak.</p>
			</figure>
			<figure class="menu-figure w-11/12 md:w-5/12 mx-auto md:mx-0">
				<div class="menu-image">
					<img src="/img/peoples/people-2.jpg" alt="Graha Wibisana" class="my-8">
				</div>
				<h2 class="font-black title-text mt-12">Brisket</h2>
				<h4 class="font-normal text-4xl mb-4">US, AUS, Wagyu</h4>
				<p class="font-normal text-2xl">Daging brisket terletak di bagian dada bawah sekitar ketiak sapi. Daging ini juga memiliki keunggulan yaitu teksturnya yang lembut karena banyak lemak.</p>
			</figure>
		</div>
	</section>
</template>

<script>
export default {
	name: 'Contact'
}
</script>

<style lang="sass">
.best-menu
	background: url('/img/backgrounds/bg-1.png') no-repeat center center scroll
	background-color: rgba(255, 255, 255, .8)
	background-blend-mode: lighten
.menu-figure
	max-width: 550px
	position: relative
.menu-image
	aspect-ratio: 1.25
	border: 5px solid #003233
	background-color: transparent
	border-radius: 128px / 128px
	transform: scale(.875)
	img
		margin: -1.25% 0 0 -6.25%
		border-radius: 128px / 128px
		position: absolute
		transform: scale(1.0625)
</style>