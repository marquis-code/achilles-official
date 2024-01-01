<template>
  <main class="w-11/12 md:w-auto container mx-auto relative">
    <div class="md:flex justify-between gap-x-20 items-center space-y-10 md:space-y-0">
      <div class="md:w-6/12">
        <img src="@/assets/img/ambassador.png" alt="" class="h-[700px] object-cover object-center w-full rounded-lg" />
      </div>
      <div class="md:w-6/12 space-y-6">
        <h1 class=" text-3xl md:text-5xl font-semibold max-w-md">Become an
          Achilles Ambassador</h1>
        <p class="md:max-w-md">Enjoy numerous perks and benefits as you
          spread the good news of Achilles Drill.</p>
        <div class="flex items-center gap-x-6">
          <button class="bg-black text-white rounded-lg font-semibold px-6 py-2.5 flex items-center space-x-4"><span>Join
              us</span> <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none"
              stroke="#ffffff" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
              <path d="M5 12h13M12 5l7 7-7 7" />
            </svg></button>
          <button class="text-black bg-gray-100 border rounded-lg font-semibold px-6 py-2.5">Learn More</button>
        </div>
      </div>
      <div class="hidden md:block">
        <img src="@/assets/icons/spiral-group.svg" alt="" class="absolute h-[700px] w-[700px] -top-40 -right-20" />
      </div>
    </div>
  </main>
</template>

<script>
export default {

}
</script>

<style></style>
