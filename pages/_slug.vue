<template>
  <article>
    <nuxt-content :document="docs" />
  </article>
</template>

<script>
export default {
  async asyncData ({ $content, params }) {
    console.log(params)
    const docs = await $content('git/git')
      .fetch()
    console.log(docs)

    // const doc = docs.filter()
    return { docs }
  }
}
</script>

<style scoped>

</style>
