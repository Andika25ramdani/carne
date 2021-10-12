<template>
  <div id="nav" class="bg-blue-200">
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link>
  </div>
  <router-view/>
</template>

<style lang="sass">
.title-text
  font-size: 4rem
  line-height: 4rem
</style>
