<template>
  <div>
    <div class="h-96 bg-black bg-opacity-90 text-white grid place-content-center">
      <div class="text-center mb-2 font-bold text-2xl">
        Order a sample
      </div>
      <div class="text-center text-xl text-purple-400 mb-8">
        If you’re a fan of feeling and seeing before you invest – we’ve got you.
      </div>
      <div class="text-xl space-y-0.5 ml-16">
        <div>1. Login to design your product</div>
        <div>2. View product in "My Collection"</div>
        <div>3. Click “Get Sample" to order your product</div>
        <div>4. Place your sample order and we do the rest!</div>
      </div>
      <div class="text-center mt-4">
        <button class="btn-primary bg-purple-400 text-bold text-xl">
          Order now
        </button>
      </div>
    </div>
    <div class="h-96 grid place-content-center gap-12 border-b-2 border-gray-800">
      <div class="font-bold text-2xl text-center">
        Need more help?
      </div>
      <div>
        <div class="flex gap-32">
          <div class="text-2xl flex flex-col items-center">
            <svg xmlns="http://www.w3.org/2000/svg" class="h-24 w-24" fill="none" viewBox="0 0 24 24" stroke="currentColor">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M8 12h.01M12 12h.01M16 12h.01M21 12c0 4.418-4.03 8-9 8a9.863 9.863 0 01-4.255-.949L3 20l1.395-3.72C3.512 15.042 3 13.574 3 12c0-4.418 4.03-8 9-8s9 3.582 9 8z" />
            </svg>
            <div class="text-2xl font-bold mt-2">
              Call us
            </div>
            <div class="font-2xl">
              1-888-918-0053
            </div>
          </div>
          <div class="text-2xl flex flex-col items-center">
            <svg xmlns="http://www.w3.org/2000/svg" class="h-24 w-24" fill="none" viewBox="0 0 24 24" stroke="currentColor">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z" />
            </svg>
            <div class="text-2xl font-bold mt-2">
              Emai us
            </div>
            <div class="font-2xl">
              help@slaitepod.com
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="h-96">
      <div class="flex justify-center gap-32 mt-16">
        <div>
          <div class="text-2xl font-bold mb-4">
            Services
          </div>
          <div v-for="(service, i) in services" :key="i" class="mb-2.5">
            <div class="hover:text-blue-400 cursor-pointer">
              {{ service }}
            </div>
          </div>
        </div>
        <div>
          <div class="text-2xl font-bold mb-4">
            Resources
          </div>
          <div v-for="(resource, i) in resources" :key="i" class="mb-2.5">
            <div class="hover:text-blue-400 cursor-pointer">
              {{ resource }}
            </div>
          </div>
        </div>
        <div>
          <div class="text-2xl font-bold mb-4">
            Features
          </div>
          <div v-for="(feature, i) in features" :key="i" class="mb-2.5">
            <div class="hover:text-blue-400 cursor-pointer">
              {{ feature }}
            </div>
          </div>
        </div>
        <div>
          <div class="text-2xl font-bold mb-4">
            Contact Us
          </div>
          <div v-for="(contact, i) in contacts" :key="i" class="mb-2.5">
            <div class="hover:text-blue-400 cursor-pointer">
              {{ contact }}
            </div>
          </div>
        </div>
      </div>
      <div class="ml-6 mt-6 text-4xl tracking-widest font-bold">
        SLAITE
      </div>
      <div class="text-center mt-10">
        © {{ new Date().getFullYear() }}. Slaite. All rights reserved.
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      services: ['Features', 'Pricing', 'Tutorials', 'Blogs', 'Help center'],
      resources: ['Dave & Buster\'s', 'Olive Garden', 'Texas Roadhouse', 'Famous Dave\'s', 'Bluepoint Sage Cafe'],
      features: ['About Us', 'Community', 'Private Policy', 'Terms of Use'],
      contacts: ['About Us', 'Community', 'Private Policy', 'Terms of Use']
    }
  }
}
</script>

<style>

</style>
