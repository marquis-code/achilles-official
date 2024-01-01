<template>
  <main class="bg-[#21272F] py-32">
    <main class="w-11/12 md:w-auto container mx-auto flex flex-col justify-between gap-y-10">
      <div class="md:flex justify-between">
        <div class="md:w-2/12">
          <img src="@/assets/icons/logo.svg" class="h-44 w-44" alt="" />
        </div>
        <div class="space-y-6 md:w-2/12">
          <div> <nuxt-link to="/" class="text-white font-medium">Lecture Banks</nuxt-link></div>
          <div> <nuxt-link to="/" class="text-white font-medium">Practice Question</nuxt-link></div>
          <div> <nuxt-link to="/" class="text-white font-medium">Ambassadors</nuxt-link></div>
          <div> <nuxt-link to="/" class="text-white font-medium">Course Rep Network</nuxt-link></div>
        </div>
        <div class="space-y-6 md:w-2/12">
          <div> <nuxt-link to="/" class="text-white font-medium">About us</nuxt-link></div>
          <div> <nuxt-link to="/" class="text-white font-medium">Partnerships</nuxt-link></div>
          <div> <nuxt-link to="/" class="text-white font-medium">Support</nuxt-link></div>
        </div>
        <div class="space-y-4 md:w-5/12">
          <h1 class="text-white font-medium">SUBSCRIBE TO OUR NEWSLETTER</h1>
          <div class="w-full md:flex justify-between items-center gap-x-3 flex-col md:flex-row space-y-4 md:space-y-0">
            <div class="md:w-10/12 space-y-2">
              <input class="py-3 rounded-lg w-full px-6 bg-white" type="email" placeholder="email@achillesdrill.com" />
              <p class="text-sm text-white font-light">Med school updates, news and education, no spam messages.</p>
            </div>
            <div class="pb-4 w-full md:w-auto">
              <button class="bg-white w-full md:w-auto text-gray-900 rounded-full text-xs px-6 py-3">Sign Up</button>
            </div>
          </div>
        </div>
      </div>
      <div class="md:flex items-center gap-x-60 space-y-10 md:space-y-0">
        <div class="flex items-center gap-x-6">
          <img src="@/assets/icons/white-twitter.svg" alt="" />
          <img src="@/assets/icons/white-facebook.svg" alt="" />
          <img src="@/assets/icons/white-instagram.svg" alt="" />
          <img src="@/assets/icons/youtube-white.svg" alt="" />
        </div>
        <div class="flex items-center gap-x-3">
          <p class="text-sm text-gray-400">Copyright © 2023 AchillesDrill</p>
          <p class="text-sm text-gray-400">Terms</p>
          <p class="text-sm text-gray-400">Privacy</p>
          <p class="text-sm text-gray-400">Cookies</p>
        </div>
      </div>
    </main>
  </main>
</template>

<script>
export default {

}
</script>

<style></style>
