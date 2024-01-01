<template>
  <main class="mt-32 lg:mt-[500px] space-y-10">
    <div class="flex justify-center items-center flex-col gap-y-2 container mx-auto">
      <h1 class="text-3xl md:text-4xl text-gray-900 font-semibold">Latest Videos</h1>
      <img src="@/assets/icons/text-spiral.svg" class="w-32" alt="" />
    </div>
    <div class="bg-[#F5F8F9] pt-20">
      <div class="container mx-auto hidden md:block">
        <ssr-carousel :slides-per-page="3" loop :autoplay-delay='3'>
          <div v-for="slide in slides" :key="slide.id" class="slide rounded-md">
            <section class="overflow-hidden bg-cover bg-top bg-no-repeat lg:h-[600px] relative">
              <div>
                <img :src="require(`@/assets/img/${slide.imgUrl}`)" class="object-center object-cover" :alt="slide.title">
              </div>
              <div class="flex justify-center items-center w-6/12 mx-auto">
                <div class="bg-black/50 rounded-lg p-3 flex justify-between items-center absolute bottom-32">
                  <div class="space-y-3">
                    <h1 class="text-lg text-white font-bold">{{ slide.title }}</h1>
                    <p class="text-white text-light max-w-xl">{{ slide.desc }}</p>
                  </div>
                  <div>
                    <img src="@/assets/icons/video-circle.svg" alt="" class="h-10 w-10" />
                  </div>
                </div>
              </div>
            </section>
          </div>
        </ssr-carousel>
      </div>
      <div class="container mx-auto md:hidden">
        <ssr-carousel :slides-per-page="1" loop :autoplay-delay='3'>
          <div v-for="slide in slides" :key="slide.id" class="slide rounded-md">
            <section class="overflow-hidden bg-cover bg-top bg-no-repeat lg:h-[600px] relative">
              <div>
                <img :src="require(`@/assets/img/${slide.imgUrl}`)" class="object-center object-cover" :alt="slide.title">
              </div>
              <div class="flex justify-center items-center">
                <div class="bg-black/50 rounded-lg p-3 flex justify-between items-center absolute bottom-20 w-11/12 mx-auto">
                  <div class="space-y-3">
                    <h1 class="text-lg text-white font-bold">{{ slide.title }}</h1>
                    <p class="text-white text-light max-w-xl text-sm">{{ slide.desc }}</p>
                  </div>
                  <div>
                    <img src="@/assets/icons/video-circle.svg" alt="" class="h-10 w-10" />
                  </div>
                </div>
              </div>
            </section>
          </div>
        </ssr-carousel>
      </div>
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
