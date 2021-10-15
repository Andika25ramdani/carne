<template>
  <div class="home">
    <Banner />
    <Begining />
    <FindUs />
    <CantVisit />
    <Available />
    <Partnership />
    <BestMenu />
    <Contact />
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import Available from '@/components/home/Available.vue'
import Banner from '@/components/home/Banner.vue'
import Begining from '@/components/home/Begining.vue'
import BestMenu from '@/components/home/BestMenu.vue'
import CantVisit from '@/components/home/CantVisit.vue'
import Contact from '@/components/home/Contact.vue'
import FindUs from '@/components/home/FindUs.vue'
import Partnership from '@/components/home/Partnership.vue'

export default {
  name: 'Home',
  components: {
    Available, Banner, Begining, BestMenu, CantVisit, Contact, FindUs, Partnership
  }
}
</script>
