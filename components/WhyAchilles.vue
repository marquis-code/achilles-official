<template>
  <main class="space-y-10 mt-32">
    <div class="flex justify-center items-center flex-col gap-y-2 container mx-auto">
      <h1 class="text-3xl md:text-4xl text-gray-900 font-semibold text-center max-w-md px-3">Why students choose Achilles Drill </h1>
      <img src="@/assets/icons/text-spiral.svg" class="w-32" alt="" />
    </div>
    <section class="md:flex justify-between w-11/12 md:w-auto container mx-auto">
      <div class="w-full md:w-6/12 space-y-6  py-10">
        <div class="space-y-6">
          <span class="bg-[#B3FBE3] py-2.5 rounded px-6">Outstanding results</span>
          <p class="text-gray-900 tracking-wide leading-loose md:max-w-md">We understand the struggles you face as a medical
            student, and we're here to provide you with the tools
            and resources you need to thrive</p>
        </div>
        <div class="space-y-6">
          <span class="bg-[#FFABE7] py-2.5 rounded px-6"> Trusted by thousands</span>
          <p class="text-gray-900 tracking-wide leading-loose md:max-w-md">We understand the struggles you face as a medical
            student, and we're here to provide you with the tools
            and resources you need to thrive</p>
        </div>
      </div>
      <div class="w-full md:w-6/12">
        <img src="@/assets/img/studying.png" alt="" class="w-full h-[500px] object-cover object-center" />
      </div>
    </section>
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
      slides: [
        {
          id: 1,
          title: 'Anatomy Of The Neurons',
          desc: 'Dive into the world of Upperlimbs and it’s structure.',
          imgUrl: 'videoImg1.png'
        },
        {
          id: 2,
          title: 'Anatomy Of The Hands',
          desc: 'Dive into the world of Upperlimbs and it’s structure.',
          imgUrl: 'videoImg3.png'
        },
        {
          id: 3,
          title: 'Anatomy Of The Legs',
          desc: 'Dive into the world of Lowerlimbs and it’s structure.',
          imgUrl: 'videoImg3.png'
        },
        {
          id: 4,
          title: 'Anatomy Of The Neurons',
          desc: 'Dive into the world of Neuroanatomy and nerves structure.',
          imgUrl: 'videoImg1.png'
        },
        {
          id: 5,
          title: 'Anatomy Of The Hands',
          desc: 'Dive into the world of Upperlimbs and it’s structure.',
          imgUrl: 'videoImg3.png'
        },
        {
          id: 6,
          title: 'Anatomy Of The Legs',
          desc: 'Dive into the world of Lowerlimbs and it’s structure.',
          imgUrl: 'videoImg3.png'
        },
        {
          id: 7,
          title: 'Anatomy Of The Neurons',
          desc: 'Dive into the world of Neuroanatomy and nerves structure.',
          imgUrl: 'videoImg1.png'
        },
        {
          id: 8,
          title: 'Anatomy Of The Hands',
          desc: 'Dive into the world of Upperlimbs and it’s structure.',
          imgUrl: 'videoImg3.png'
        },
        {
          id: 9,
          title: 'Anatomy Of The Legs',
          desc: 'Dive into the world of Lowerlimbs and it’s structure.',
          imgUrl: 'videoImg3.png'
        }
      ]
    }
  }
}
</script>

<style></style>
