<template>
	<div class="text-white bg-green pb-16">
		<h2 class="font-black text-center title-text pt-8 pb-6">Contact</h2>
		<div class="flex flex-1 flex-col md:flex-row justify-evenly gap-y-16 mx-auto">
			<figure class="contact-figure w-11/12 sm:w-10/12 md:w-5/12 mx-auto md:mx-0">
				<img src="/img/peoples/people-1.jpg" alt="Ghani Husnan Afdhaluddin" class="contact-image-person my-8">
				<h2 class="font-black title-text">Ghani Husnan Afdhaluddin</h2>
				<h3 class="text-5xl font-medium">Co-Founder & CEO</h3>
				<a href="tel:+6282121643817">
					<h4 class="font-normal text-4xl">0821 2164 3817</h4>
				</a>
			</figure>
			<figure class="contact-figure w-11/12 md:w-5/12 mx-auto md:mx-0">
				<img src="/img/peoples/people-2.jpg" alt="Graha Wibisana" class="contact-image-person my-8">
				<h2 class="font-black title-text">Graha<br>Wibisana</h2>
				<h3 class="text-5xl font-medium">Co-Founder & CEO</h3>
				<a href="tel:+6282121643817">
					<h4 class="font-normal text-4xl">0821 2164 3817</h4>
				</a>
			</figure>
		</div>
	</div>
</template>

<script>
export default {
	name: 'Contact'
}
</script>

<style lang="sass">
.contact-figure
	max-width: 601px
	h1, h2, h3, h4
		line-height: 4rem
		text-align: left
		@media screen and (min-width: 0)
			transform: scale(.75)
		@media screen and (min-width: 400)
			transform: scale(.875)
		@media screen and (min-width: 640px)
			transform: scale(1)
		@media screen and (min-width: 768px)
			transform: scale(.875)
		@media screen and (min-width: 1024px)
			transform: scale(1)
img.contact-image-person
	aspect-ratio: 1.32
	width: 100%
	max-height: 452px
</style>