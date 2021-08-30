<template>
  <nav class="sticky top-0 z-50 w-full flex flex-row items-center justify-between h-12">
    <nuxt-link to="/" class="flex flex-row pl-2 md:pl-8">
      <img src="~/static/icon.png" alt="app-logo" class="w-10 mr-2 pt-2 text-justify">
      <!-- <strong class="text-3xl font-serif items-center flex">
        {{ appTitle }}
      </strong> -->
    </nuxt-link>
    <search-bar />
    <div class="hidden md:flex md:flex-row h-full justify-center items-center pr-8">
      <nuxt-link to="/about" class="">
        About
      </nuxt-link>
    </div>
  </nav>
</template>

<script>
export default {
  props: {
    appTitle: {
      type: String,
      default: 'App'
    }
  }
}
</script>

<style>
</style>
