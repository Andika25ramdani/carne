<template>
  <section class="contact text-white bg-green">
		<div v-if="contentActive" class="grid grid-cols-1 sm:grid-cols-2 gap-8 sm:gap-16 items-center w-2/3 sm:w-5/6 mx-auto py-8 sm:py-12 md:py-16 lg:py-20 xl:py24 2xl:py-28">
      <transition-group name="slide-up" appear>
        <img v-for="activity in activities" :key=activity.id :src=activity.img :alt=activity.imgAlt>
      </transition-group>
		</div>
	</section>
</template>

<script>
export default {
  name: 'Activity',
  data() {
    return {
      contentActive: false,
      activities: [
        {
          id: 1,
          img: '/img/peoples/1.png',
          imgAlt: 'Activity 1'
        },
        {
          id: 2,
          img: '/img/peoples/2.png',
          imgAlt: 'Activity 2'
        },
        {
          id: 3,
          img: '/img/peoples/3.png',
          imgAlt: 'Activity 3'
        },
        {
          id: 4,
          img: '/img/peoples/3.png',
          imgAlt: 'Activity 3'
        },
      ]
    }
  },
  mounted() {
    this.contentActive = true
  }
}
</script>

<style lang="sass">
</style>