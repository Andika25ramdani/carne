<template>
  <section class="home-banner text-white text-center h-screen flex flex-col justify-center align-center">
    <transition-group name="slide-up" appear>
      <h2 v-if="contentActive" class="font-black title-text pb-8">THE BEST SMOKED<br>BBQ IN TOWN</h2>
      <p v-if="contentActive" class="font-normal text-default mx-auto w-11/12 xl:w-10/12 2xl:w-9/12">
        Let The Taste Speak For It Self
      </p>
    </transition-group>
	</section>
</template>

<script>
export default {
  name: 'Banner',
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
.home-banner
  background: url('/img/backgrounds/1.jpg') no-repeat center center scroll
</style>