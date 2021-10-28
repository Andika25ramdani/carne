<template>
	<section class="contact text-white bg-green py-16">
		<transition name="slide-up">
			<h2 v-if="contentActive" class="font-black text-center title-text pb-6">Contact</h2>
		</transition>
		<div class="flex flex-1 flex-col sm:flex-row justify-evenly gap-y-8 sm:gap-y-16 mx-auto">
			<figure v-for="contact in contacts" :key=contact.id class="contact-figure w-7/12 sm:w-5/12 mx-auto sm:mx-0">
				<img :src=contact.img :alt=contact.name class="contact-image-person my-4 sm:my-8">
				<h2 class="font-black title-text">{{ contact.name }}</h2>
				<h3 class="subtitle-text font-medium">{{ contact.post }}</h3>
				<a :href="'tel:+62'+contact.phone">
					<h4 class="font-normal text-default">0{{ contact.phone }}</h4>
				</a>
			</figure>
		</div>
	</section>
</template>

<script>
export default {
	name: 'Contact',
	data(){
		return{
			contentActive: false,
			contacts: [
				{
					id: 1,
					img: '/img/peoples/people-1.jpg',
					name: 'Ghani Husnan Afdhaluddin',
					post: 'Co-Founder & CEO',
					phone: '82121643817'
				},
				{
					id: 2,
					img: '/img/peoples/people-2.jpg',
					name: 'Graha Wibisana',
					post: 'Co-Founder & CEO',
					phone: '81223262607'
				}
			]
		}
	},
	mounted(){
		this.contentActive = true
	}
}
</script>

<style lang="sass">
.contact-figure
	max-width: 601px
	// h1, h2, h3, h4
	// 	line-height: 4rem
	// 	text-align: left
	// 	@media screen and (min-width: 0)
	// 		transform: scale(.75)
	// 	@media screen and (min-width: 400)
	// 		transform: scale(.875)
	// 	@media screen and (min-width: 640px)
	// 		transform: scale(1)
	// 	@media screen and (min-width: 768px)
	// 		transform: scale(.875)
	// 	@media screen and (min-width: 1024px)
	// 		transform: scale(1)
img.contact-image-person
	aspect-ratio: 1.32
	border-radius: 25% / 25%
	width: 100%
	max-height: 452px
</style>