<template>
  <main class="bg-[#F5F8F9] py-20 my-20">
    <div class="hidden md:block container mx-auto">
      <ssr-carousel :slides-per-page="4" class="">
        <div v-for="(itm, idx) in questions" :key="idx" class="bg-white rounded-md shadow-md p-10 slide">
          <img src="@/assets/icons/quotation.svg" alt="" class="h-10 w-10" />
          <p class="text-gray-500">{{ itm }}</p>
        </div>
      </ssr-carousel>
    </div>
    <div class="md:hidden container mx-auto w-11/12 md:w-auto">
      <ssr-carousel :slides-per-page="1" class="">
        <div v-for="(itm, idx) in questions" :key="idx" class="bg-white rounded-md shadow-md p-10 slide">
          <img src="@/assets/icons/quotation.svg" alt="" class="h-10 w-10" />
          <p class="text-gray-500">{{ itm }}</p>
        </div>
      </ssr-carousel>
    </div>
  </main>
</template>

<script>
import SsrCarousel from 'vue-ssr-carousel'
import ssrCarouselCss from 'vue-ssr-carousel/index.css'
export default {
  components: {
    SsrCarousel
  },
  data() {
    return {
      questions: ['Anatomy is after my life, help!', 'How can I read better as a student?', 'Biochemistry has been stressing my life.', 'Physiology is after my how do I study?', 'Anatomy is after my life, help!', 'How can I read better as a student?', 'Biochemistry has been stressing my life.', 'Physiology is after my how do I study?']
    }
  }
}
</script>

<style></style>
