<template>
  <div class="home">
    <Begining />
    <FindUs />
    <BestMenu />
    <Contact />
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import Begining from '@/components/home/Begining.vue'
import BestMenu from '@/components/home/BestMenu.vue'
import Contact from '@/components/home/Contact.vue'
import FindUs from '@/components/home/FindUs.vue'

export default {
  name: 'Home',
  components: {
    Begining, BestMenu, Contact, FindUs
  }
}
</script>
