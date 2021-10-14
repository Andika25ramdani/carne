<template>
  <section class="find-us text-white pb-16">
    <h2 class="font-black text-center title-text pt-8 pb-16">Where To Find Us?</h2>
		<div class="flex flex-1 flex-col md:flex-row justify-evenly gap-y-16 mx-auto">
			<figure class="loc-figure w-11/12 md:w-5/12 mx-auto md:mx-0">
				<div class="loc-image">
					<img src="/img/backgrounds/bg-2.jfif" alt="Graha Wibisana" class="my-8">
					<!-- <img src="https://betterstudio.com/wp-content/uploads/2019/05/1-1-instagram-1024x1024.jpg" alt="Graha Wibisana" class=""> -->
          <div class="loc-desc">
            <h2 class="font-black title-text">Bandung</h2>
            <h4 class="font-normal text-4xl">Jl. Aceh No. 45 <br> Mon - Sun <br>11.00 - 20.00</h4>
          </div>
				</div>
			</figure>
			<figure class="loc-figure w-11/12 md:w-5/12 mx-auto md:mx-0">
				<div class="loc-image">
					<img src="/img/backgrounds/bg-3.jfif" alt="Graha Wibisana" class="my-8">
					<!-- <img src="https://betterstudio.com/wp-content/uploads/2019/05/1-1-instagram-1024x1024.jpg" alt="Graha Wibisana" class=""> -->
          <div class="loc-desc">
            <h2 class="font-black title-text">Bandung</h2>
            <h4 class="font-normal text-4xl">Jl. Karasak No. 109 <br> Mon - Sun <br>11.00 - 20.00</h4>
          </div>
				</div>
			</figure>
		</div>
  </section>
</template>

<script>
export default {
	name: 'FindUs'
}
</script>

<style lang="sass">
.find-us
	background: url('/img/backgrounds/bg-4.png') no-repeat center center scroll
	background-color: rgba(0, 50, 51, .9)
	background-blend-mode: hard-light
.loc-figure
	max-width: 683px
	position: relative
.loc-image
	aspect-ratio: 1
	border: 4px solid white
	background-color: transparent
	border-radius: 183px / 183px
	transform: scale(.875)
  position: relative
	img
		margin: -6.25% 0 0 -6.25%
		border-radius: 183px / 183px
		position: absolute
		transform: scale(1.0625)
.loc-desc
  margin: -6.25% 12.5% auto
  position: absolute
  display: flex
  flex-direction: column
  justify-content: center
  height: 100%
</style>