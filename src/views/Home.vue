<template>
  <div class="home">
    <BestMenu />
    <Contact />
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import BestMenu from '@/components/home/BestMenu.vue'
import Contact from '@/components/home/Contact.vue'

export default {
  name: 'Home',
  components: {
    BestMenu, Contact
  }
}
</script>
