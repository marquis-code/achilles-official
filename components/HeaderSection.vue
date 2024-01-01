<template>
  <header class="bg-[#27396B] h-screen relative">
    <div class="mx-auto max-w-screen-2xl px-4 sm:px-6 lg:px-8">
      <div class="flex h-32 items-center justify-between">
        <div class="hidden md:block">
          <nav aria-label="Global">
            <ul class="flex items-center gap-6 text-sm">
              <li>
                <a
                  class="text-white transition hover:text-gray-500/75"
                  href="/"
                >
                  About
                </a>
              </li>

              <li>
                <a
                  class="text-white transition hover:text-gray-500/75"
                  href="/"
                >
                  Careers
                </a>
              </li>

              <li>
                <a
                  class="text-white transition hover:text-gray-500/75"
                  href="/"
                >
                  History
                </a>
              </li>

              <li>
                <a
                  class="text-white transition hover:text-gray-500/75"
                  href="/"
                >
                  Services
                </a>
              </li>

              <li>
                <a
                  class="text-white transition hover:text-gray-500/75"
                  href="/"
                >
                  Projects
                </a>
              </li>

              <li>
                <a
                  class="text-white transition hover:text-gray-500/75"
                  href="/"
                >
                  Blog
                </a>
              </li>
            </ul>
          </nav>
        </div>
        <div class="md:flex md:items-center md:gap-12">
          <a class="block text-teal-600" href="/">
            <span class="sr-only">Home</span>
            <img src="@/assets/icons/logo.svg" alt="" />
          </a>
        </div>

        <div class="flex items-center gap-4">
          <div class="hidden lg:flex sm:gap-4">
            <div class="pt-2">
              <a class="text-sm font-medium text-white" href="/"> Login </a>
            </div>

            <div class="hidden sm:flex">
              <a
                class="rounded-md bg-[#21272F] px-5 py-2.5 text-sm font-medium text-white"
                href="/"
              >
                Register
              </a>
            </div>
          </div>

          <div class="block md:hidden">
            <button class="">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                width="25"
                height="25"
                viewBox="0 0 24 24"
                fill="none"
                stroke="#000000"
                stroke-width="2.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              >
                <line x1="3" y1="12" x2="21" y2="12"></line>
                <line x1="3" y1="6" x2="21" y2="6"></line>
                <line x1="3" y1="18" x2="21" y2="18"></line>
              </svg>
            </button>
          </div>
        </div>
      </div>
    </div>
    <main class="mt-20 md:pt-32 w-11/12 mx-auto md:w-auto">
      <div class="flex justify-center items-center flex-col space-y-6">
        <h1
          class="leading-loosed tracking-widest text-3xl md:text-6xl font-semibold md:max-w-2xl text-white text-center animate__animated animate__rotateIn"
        >
          We’ve Finally Hacked Med-school!
        </h1>
        <p
          class="font-light text-white text-center animate__animated animate__rotateIn"
        >
          Connect with a community of medical student learning from our
          resources.
        </p>
        <buuton class="bg-[#21272F] text-white rounded-full px-6 py-3"
          >Start learning</buuton
        >
      </div>
      <div class="absolute bottom-0 inset-x-10 z-10 hidden md:block">
        <img src="@/assets/icons/colored-stripe.svg" alt="" class="z-10" />
      </div>
    </main>
    <div class="flex justify-center items-center relative">
      <div
        v-if="$nuxt.isOffline"
        class="w-10/12 mx-auto z-50 absolute -bottom-96 md:-bottom-[800px]"
      >
        <img src="@/assets/img/cardavar.png" alt="" class="z-50 h-60 md:h-auto" />
      </div>
      <div class="flex justify-center items-center" v-if="!$nuxt.isOffline">
        <div
          class="z-50 absolute top-52 rounded-md hidden md:block"
        >
          <iframe
            width="1000"
            height="600"
            src="https://www.youtube.com/embed/lToIUS5ITp4?si=orVq7i23nC_iKcVd"
            title="YouTube video player"
            frameborder="0"
            allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
            allowfullscreen
          ></iframe>
        </div>
        <div
        class="z-50 absolute top-32 rounded-md md:hidden"
      >
        <iframe
          width="100%"
          height="400"
          src="https://www.youtube.com/embed/lToIUS5ITp4?si=orVq7i23nC_iKcVd"
          title="YouTube video player"
          frameborder="0"
          allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
          allowfullscreen
        ></iframe>
      </div>
      </div>
    </div>
  </header>
</template>

<script >
export default {
  data() {
    return {
      paths: [
        {
          name: "Lecture Banks",
          url: "#",
        },
        {
          name: "Practice Questions",
          url: "#",
        },
        {
          name: "Ambassadors",
          url: "#",
        },
        {
          name: "Courses",
          url: "#",
        },
      ],
    };
  },
};
</script>
