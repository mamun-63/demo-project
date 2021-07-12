<template>
  <div class="default-text">
    <Navbar />
    <div class="bg-gradient-to-r from-red-500 h-12" />
    <div class="h-32 bg-gray-200 mb-14 text-black flex flex-col items-center justify-center">
      <div class="font-bold text-4xl">
        Product Catalogue
      </div>
      <div class="text-xl">
        View our assortment of high-quality products and brands
      </div>
    </div>
    <div class="text-center grid grid-cols-9 mb-16">
      <input class="input-simple col-start-4 col-span-3 text-sm italic" type="text" placeholder="Search for products, brands, categories">
    </div>
    <div class="mx-64 grid grid-cols-3 gap-6 place-content-center">
      <div v-for="i in 3" :key="i" class="shadow-lg border w-full h-64">
        <div class="flex items-center justify-center h-full">
          <div class="text-xl flex items-center justify-center font-bold bg-gray-300 h-48 w-8/12">
            T-shirts
          </div>
        </div>
      </div>
    </div>
    <div>
      <Footer />
    </div>
  </div>
</template>

<script>
import Footer from '~/components/Footer.vue'
export default {
  components: { Footer }

}
</script>

<style>

</style>
