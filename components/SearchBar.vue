<template>
  <div class="bg-white flex items-center rounded-lg border-2 w-full mx-8">
    <input
      class="w-full py-2 px-4 text-gray-700 leading-tight focus:outline-none"
      type="search"
      name="search"
      placeholder="Search"
    >
    <div>
      <button type="submit" class="text-gray-500 rounded-full p-2 pr-4 hover:text-gray-800 focus:outline-none w-8 h-8 flex items-center justify-center">
        <search-icon />
      </button>
    </div>
  </div>
</template>

<script>
import SearchIcon from './SearchIcon.vue'
export default { components: { SearchIcon } }
</script>

<style scoped>

</style>
