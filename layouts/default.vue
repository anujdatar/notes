<template>
  <div>
    <notes-header :app-title="appTitle" />
    <Nuxt />
  </div>
</template>

<script>
export default {
  data () {
    return {
      appTitle: 'Nuxt-Notes'
    }
  }
}
</script>

<style>
</style>
