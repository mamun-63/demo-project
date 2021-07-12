<template>
  <div class="default-text">
    <div class="shadow-md h-32 flex justify-between">
      <div class="flex items-center ml-3 md:ml-24">
        <div class="text-7xl font-bold mr-12">
          S
        </div>
        <div v-for="(item, i) in items" :key="i" class="ml-5">
          <div class="cursor-pointer hover:text-blue-500 text-md uppercase leading-4 tracking-wider font-light">
            {{ item }}
          </div>
        </div>
      </div>
      <div class="flex items-center gap-3 mr-3 md:mr-24">
        <button class="btn-outlined">
          Sing in
        </button>
        <button class="btn-primary">
          Sing up
        </button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      items: ['About', 'Slaite', 'How it works', 'Catalog', 'blog', 'Integrations', 'FAQ']
    }
  }
}
</script>

<style>

</style>
