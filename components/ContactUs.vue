<template>
  <main class="container mx-auto my-32 w-11/12 md:w-auto">
    <div class="md:flex justify-between gap-x-32 space-y-10 md;space-y-0">
      <div class="md:w-6/12 space-y-6">
        <div class="space-y-4">
          <h1 class="text-4xl md:text-5xl font-semibold max-w-lg">We’ll love to keep in touch with you.</h1>
          <p class="text-gray-600 font-light">You can reach out to us through the link below</p>
        </div>
        <div class="space-y-4 rounded-lg p-6 bg-gradient-to-r from-indigo-500 via-purple-500 to-pink-500 md:w-6/12">
          <img src="@/assets/icons/envelope.svg" alt="" />
          <p class="text-sm text-gray-900">Email Address</p>
          <p class="font-bold">achillesdrill@gmail.com</p>
        </div>
        <div class="space-y-6">
          <div class="flex items-center gap-x-2">
            <img src="@/assets/icons/line.svg" alt="" />
            <p class="font-bold">Connect with us:</p>
          </div>
          <div class="flex items-center gap-x-3">
            <img src="@/assets/icons/whatsapp.svg" class="h-14 w-14" alt="" />
            <img src="@/assets/icons/instagram.svg" class="h-14 w-14" alt="" />
            <img src="@/assets/icons/twitter.svg" class="rounded-full" alt="" />
            <img src="@/assets/icons/Youtube.svg" alt="" />
            <img src="@/assets/icons/telegram.svg" alt="" />
          </div>
        </div>
      </div>
      <div class="md:w-6/12">
        <form class="p-6 md:p-10 bg-white shadow-md border-[0.4px] rounded-3xl space-y-6">
          <h1 class="text-xl md:text-4xl font-medium">Contact us</h1>
          <div class="w-full">
            <label class="text-sm text-gray-700 md:text-lg font-medium">Name</label>
            <input type="text" placeholder="Bayo Samuel" class="w-full text-sm outline-none px-6 border py-3 rounded-md" />
          </div>
          <div class="w-full">
            <label class="text-sm text-gray-700 md:text-lg font-medium">Email</label>
            <input type="text" placeholder="bayosamuel@gmail.com"
              class="w-full text-sm outline-none px-6 border py-3 rounded-md" />
          </div>
          <div class="w-full">
            <label class="text-sm text-gray-700 md:text-lg font-medium">Subject</label>
            <input type="text" placeholder="Achilles Lecture Banks"
              class="w-full text-sm outline-none px-6 border py-3 rounded-md" />
          </div>
          <div class="w-full">
            <label class="text-sm text-gray-700 md:text-lg font-medium">Message</label>
            <textarea placeholder="Tell us about your....."
              class="w-full text-sm px-6 py-3 outline-none resize-none border rounded-md" cols="6" rows="6" />
          </div>
          <div class="flex justify-end items-end">
            <button class="text-gray-900 px-6 py-2.5 font-semibold bg-gray-100 rounded-full">Send</button>
          </div>
        </form>
      </div>
    </div>
  </main>
</template>

<script>
export default {

}
</script>

<style></style>
