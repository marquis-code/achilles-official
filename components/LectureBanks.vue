<template>
  <main class="relative container w-11/12 mx-auto md:w-auto">
    <div>
      <div class="flex justify-center items-center">
        <h1 class="text-4xl md:text-6xl font-light text-center max-w-5xl leading-loose tracking-wide">We’ve heard every
          need and.....
          ........we have the <span class="font-bold">SOLUTIONS!</span> </h1>
      </div>
    </div>
    <div class="absolute top-24 right-96">
      <img src="@/assets/icons/circular-stripe.svg" alt="" />
    </div>
    <div class="flex justify-center items-center flex-col gap-y-2 container mx-auto mt-20 md:mt-32">
      <h1 class="text-3xl md:text-4xl text-gray-900 font-semibold text-center max-w-3xl">Lecture Banks</h1>
      <img src="@/assets/icons/text-spiral.svg" class="w-32" alt="" />
      <p class="text-gray-600 md:text-lg max-w-2xl text-sm text-center">Stay ahead of the class when you use our
        pre-recorded bank of over 400 tutorial
        videos
        on Anatomy, Physiology and biochemistry, you can:</p>
    </div>
    <div class="md:flex justify-between mt-10 space-y-6 md:-space-y-0">
      <div class="space-y-6 md:w-6/12 w-full hidden md:block">
        <div v-for="(itm, idx) in lectureBanks" :key="idx" class="flex gap-x-6">
          <div>
            <img :src="require(`@/assets/icons/${itm.imgUrl}`)" alt="" />
          </div>
          <div class="space-y-2">
            <h1 class="font-bold text-xl md:text-2xl">{{ itm.title }}</h1>
            <p class="text-gray-700 leading-relaxed">{{ itm.desc }}</p>
          </div>
        </div>
      </div>
      <div class="space-y-6 md:w-6/12 w-full md:hidden ">
        <div v-for="(itm, idx) in lectureBanks" :key="idx" class="flex flex-col justify-center items-center gap-y-4">
          <div>
            <img :src="require(`@/assets/icons/${itm.imgUrl}`)" alt="" />
          </div>
          <div class="flex flex-col justify-center items-center gap-y-3">
            <h1 class="font-bold text-xl md:text-2xl text-center">{{ itm.title }}</h1>
            <p class="text-gray-700 leading-relaxed text-center">{{ itm.desc }}</p>
          </div>
        </div>
      </div>
      <div class="md:w-6/12 relative w-full">
        <ssr-carousel loop :autoplay-delay='3'>
          <div class="slide relative" v-for="(itm, idx) in caroselList" :key="idx">
            <img src="@/assets/img/banks.png" alt="" class="h-[400px] md:h-full object-cover object-center rounded-lg" />
            <div class="absolute top-14 left-10 space-y-10 md:space-y-14">
              <span class="rounded-full px-3 py-2.5 bg-[#6BDDC0] text-[#3D3D4E] text-sm">{{ itm.tag }}</span>
              <div class="space-y-4">
                <h1 class="text-2xl md:text-6xl font-semibold text-white max-w-xl">{{ itm.title }}</h1>
                <p class="font-light text-sm md:text-lg text-white max-w-sm">{{ itm.desc }}</p>
              </div>
              <button class="text-white bg-black px-6 py-2 rounded-full">Get started</button>
            </div>
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
      lectureBanks: [
        {
          title: '1. Learn at your pace',
          desc: 'Study and progress at your own speed.',
          imgUrl: 'award.svg'
        },
        {
          title: '2. 24hrs support team',
          desc: 'Assistance and service available around the clock.',
          imgUrl: 'security-user.svg'
        },
        {
          title: '3. Access to quality content',
          desc: 'The contents are informed and empowering experiences.',
          imgUrl: 'access.svg'
        }
      ],
      caroselList: [
        {
          title: 'Anatomy lecture bank',
          desc: 'Study the structure and organization of the human body.',
          tag: 'Study body parts!'
        },
        {
          title: 'Anatomy lecture bank',
          desc: 'Study the structure and organization of the human body.',
          tag: 'Study body parts!'
        },
        {
          title: 'Anatomy lecture bank',
          desc: 'Study the structure and organization of the human body.',
          tag: 'Study body parts!'
        },
        {
          title: 'Anatomy lecture bank',
          desc: 'Study the structure and organization of the human body.',
          tag: 'Study body parts!'
        },
        {
          title: 'Anatomy lecture bank',
          desc: 'Study the structure and organization of the human body.',
          tag: 'Study body parts!'
        }
      ]
    }
  }
}
</script>

