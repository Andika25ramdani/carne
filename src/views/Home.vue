<template>
  <div class="home">
    <FindUs />
    <BestMenu />
    <Contact />
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import BestMenu from '@/components/home/BestMenu.vue'
import Contact from '@/components/home/Contact.vue'
import FindUs from '@/components/home/FindUs.vue'

export default {
  name: 'Home',
  components: {
    BestMenu, Contact, FindUs
  }
}
</script>
