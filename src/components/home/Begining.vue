<template>
  <section class="begining text-green text-center pt-8 pb-16">
    <transition-group name="slide-up" appear>
			<h2 v-if="contentActive" class="font-black title-text py-8">The Begining</h2>
			<p v-if="contentActive" class="font-normal text-default mx-auto w-11/12 xl:w-10/12 2xl:w-9/12">
				Berawal dari hobi Ghani Husnan Afdhaluddin (owner) memasak steak, yg awalnya hanya untuk sekedar menyajikannya kepada teman-teman. Ghani merasa bosan dengan steak dan berinovasi membuat smoked BBQ. Ghani melihat adanya peluang untuk menciptakan bisnis kuliner Smoked BBQ bernama Carne Smoked BBQ.  Awal mulanya Carne berdiri, bertempat di halaman rumah ( Jalan Karasak no. 109 ) dengan sistim Pre Order. Akhirnya Carne memperluas jangkauan dengan GoFood & GrabFood. Seiring dengan kesuksesan Carne, pada bulan Agustus 2021, Carne mendirikan cabang baru di Jalan Aceh no. 45
			</p>
		</transition-group>
	</section>
</template>

<script>
export default {
	name: 'Begining',
  data() {
    return {
      contentActive: false
    }
  },
	mounted () {
		this.contentActive = true
	}
}
</script>

<style lang="sass">
.begining
	background: url('/img/backgrounds/2.png') no-repeat center center scroll
	background-color: rgba(255, 255, 255, .7)
	background-blend-mode: lighten
</style>