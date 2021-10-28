<template>
  <section class="partnership text-green pb-16">
    <transition name="slide-up" appear>
      <h2 v-if="partnerTitle" class="font-black text-center title-text pt-8 pb-16">Who Have Worked With Us Before?</h2>
		</transition>
    <ul v-if="contentActive" class="grid grid-cols-1 sm:grid-cols-2 gap-y-8 sm:gap-y-16 items-center w-2/3 sm:w-5/6 mx-auto">
      <transition-group name="slide-up" appear>
        <li v-for="partner in partners" :key=partner.id>
          <a :href=partner.url target="_blank" rel="noopener noreferrer">
            <img :src=partner.img :alt=partner.imgAlt>
          </a>
        </li>
      </transition-group>
    </ul>
	</section>
</template>

<script>
export default {
  name: 'Partnership',
  data() {
    return {
			partnerTitle: false,
      contentActive: false,
      partners: [
        {
          id: 1,
          url: 'https://',
          img: '/img/partners/roots.png',
          imgAlt: 'Roots',
          hover: true,
        },
        {
          id: 2,
          url: 'https://',
          img: '/img/partners/jimmyandmartin.png',
          imgAlt: 'Jimmy And Martin',
          hover: true,
        },
        {
          id: 3,
          url: 'https://',
          img: '/img/partners/memento.png',
          imgAlt: 'Memento Coffee',
          hover: true,
        },
        {
          id: 4,
          url: 'https://',
          img: '/img/partners/pizzaplace.png',
          imgAlt: 'Pizza Place',
          hover: true,
        },
      ]
    }
  },
	mounted () {
		this.partnerTitle = true
    this.contentActive = true
	}
}
</script>

<style lang="sass">
.partnership img
  width: 100%
  max-width: 345px
  height: 100%
  margin: 0 auto
</style>