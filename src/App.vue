<template>
  <div id="nav" class="bg-blue-200">
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link>
  </div>
  <router-view/>
</template>

<style lang="sass">
h2.title-text
  font-size: 1.3rem
  line-height: 1.3rem
  @media screen and (min-width: 640px)
    font-size: 1.4rem
    line-height: 1.4rem
  @media screen and (min-width: 768px)
    font-size: 1.8rem
    line-height: 1.8rem
  @media screen and (min-width: 1024px)
    font-size: 2.5rem
    line-height: 2.5rem
  @media screen and (min-width: 1280px)
    font-size: 3.2rem
    line-height: 3.2rem
  @media screen and (min-width: 1536px)
    font-size: 4rem
    line-height: 4rem
.subtitle-text
  font-size: .975rem
  line-height: .975rem
  @media screen and (min-width: 768px)
    font-size: 1.5rem
    line-height: 1.5rem
  @media screen and (min-width: 1024px)
    font-size: 1.9rem
    line-height: 1.9rem
  @media screen and (min-width: 1280px)
    font-size: 2.5rem
    line-height: 2.5rem
  @media screen and (min-width: 1536px)
    font-size: 3rem
    line-height: 3rem
.text-default
  font-size: .73125rem
  line-height: .73125rem
  @media screen and (min-width: 640px)
    font-size: .9rem
    line-height: .9rem
  @media screen and (min-width: 768px)
    font-size: 1.1rem
    line-height: 1.1rem
  @media screen and (min-width: 1024px)
    font-size: 1.4rem
    line-height: 1.4rem
  @media screen and (min-width: 1280px)
    font-size: 1.6rem
    line-height: 1.6rem
  @media screen and (min-width: 1536px)
    font-size: 2.25rem
    line-height: 2.25rem
.text-small
  font-size: .66875rem
  line-height: .66875rem
  @media screen and (min-width: 640px)
    font-size: .8375rem
    line-height: .8375rem
  @media screen and (min-width: 768px)
    font-size: .975rem
    line-height: .975rem
  @media screen and (min-width: 1024px)
    font-size: 1.15rem
    line-height: 1.15rem
  @media screen and (min-width: 1280px)
    font-size: 1.35rem
    line-height: 1.35rem
  @media screen and (min-width: 1536px)
    font-size: 1.5rem
    line-height: 1.5rem
</style>
