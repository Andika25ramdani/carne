<template>
  <div class="home">
    <Contact />
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import Contact from '@/components/home/Contact.vue'

export default {
  name: 'Home',
  components: {
    Contact
  }
}
</script>
