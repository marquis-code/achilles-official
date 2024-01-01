<template>
  <section class="container mx-auto space-y-20">
    <div class="flex justify-center items-center flex-col gap-y-2 container mx-auto">
      <h1 class="text-2xl md:text-4xl text-gray-900 font-semibold text-center">Reviews From Students</h1>
      <img src="@/assets/icons/underline.svg" class="w-32" alt="" />
    </div>
    <div class="hidden md:block">
      <ssr-carousel :slides-per-page="4">
        <div v-for="(itm, idx) in reviews" :key="idx" class="border-8 rounded-2xl p-6 bg-white space-y-6"
          :class="itm.color">
          <img src="@/assets/icons/purples-exclamation.svg" alt="" />
          <p class="text-[#061C3D]">{{ itm.desc }}</p>
          <div class="flex items-center gap-x-3">
            <div><img :src="require(`@/assets/img/${itm.avatar}`)" alt="" class="h-10 w-10" /></div>
            <div>
              <h1 class="font-bold">{{ itm.name }}</h1>
              <p class="text-sm text-gray-700">{{ itm.dept }}</p>
            </div>
          </div>
        </div>
      </ssr-carousel>
    </div>
    <div class="md:hidden w-11/12 mx-auto">
      <ssr-carousel :slides-per-page="1" loop :autoplay-delay='3'>
        <div v-for="(itm, idx) in reviews" :key="idx" class="border-8 rounded-2xl p-6 bg-white space-y-6"
          :class="itm.color">
          <img src="@/assets/icons/purples-exclamation.svg" alt="" />
          <p class="text-[#061C3D]">{{ itm.desc }}</p>
          <div class="flex items-center gap-x-3">
            <div><img :src="require(`@/assets/img/${itm.avatar}`)" alt="" class="h-10 w-10" /></div>
            <div>
              <h1 class="font-bold">{{ itm.name }}</h1>
              <p class="text-sm text-gray-700">{{ itm.dept }}</p>
            </div>
          </div>
        </div>
      </ssr-carousel>
    </div>
  </section>
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
      reviews: [
        {
          desc: `Achilles Drill is the best thing that
ever happened to me in Med-school.
I am truly happy that I discovered
Achilles Drill.`,
          name: 'Eddie James',
          dept: 'BDS, Lagos.',
          avatar: 'avatar.png',
          color: 'border-[#FFE6CB]'
        },
        {
          desc: `Achilles Drill is the best thing that
ever happened to me in Med-school.
I am truly happy that I discovered
Achilles Drill.`,
          name: 'Eddie James',
          dept: 'BDS, Lagos.',
          avatar: 'avatar.png',
          color: 'border-[#FCDBF4]'
        },
        {
          desc: `Achilles Drill is the best thing that
ever happened to me in Med-school.
I am truly happy that I discovered
Achilles Drill.`,
          name: 'Eddie James',
          dept: 'BDS, Lagos.',
          avatar: 'avatar.png',
          color: 'border-[#F249C8]'
        },
        {
          desc: `Achilles Drill is the best thing that
ever happened to me in Med-school.
I am truly happy that I discovered
Achilles Drill.`,
          name: 'Eddie James',
          dept: 'BDS, Lagos.',
          avatar: 'avatar.png',
          color: 'border-[#FFE6CB]'
        },
        {
          desc: `Achilles Drill is the best thing that
ever happened to me in Med-school.
I am truly happy that I discovered
Achilles Drill.`,
          name: 'Eddie James',
          dept: 'BDS, Lagos.',
          avatar: 'avatar.png',
          color: 'border-[#FFE6CB]'
        },
        {
          desc: `Achilles Drill is the best thing that
ever happened to me in Med-school.
I am truly happy that I discovered
Achilles Drill.`,
          name: 'Eddie James',
          dept: 'BDS, Lagos.',
          avatar: 'avatar.png',
          color: 'bgorder[#FCDBF4]'
        },
        {
          desc: `Achilles Drill is the best thing that
ever happened to me in Med-school.
I am truly happy that I discovered
Achilles Drill.`,
          name: 'Eddie James',
          dept: 'BDS, Lagos.',
          avatar: 'avatar.png',
          color: 'border-[#FCDBF4]'
        },
        {
          desc: `Achilles Drill is the best thing that
ever happened to me in Med-school.
I am truly happy that I discovered
Achilles Drill.`,
          name: 'Eddie James',
          dept: 'BDS, Lagos.',
          avatar: 'avatar.png',
          color: 'border-[#FCDBF4]'
        }
      ]
    }
  }
}
</script>

<style></style>
