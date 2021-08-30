<template>
  <div>
    Homepage
  </div>
</template>

<script>
export default {
  async asyncData ({ $content, params }) {
    console.log(params.slug)
    const articles = await $content('', { deep: true }, params.path)
      .sortBy('createdAt', 'asc')
      .fetch()
    console.log(articles)
    return { articles }
  }
}
</script>
