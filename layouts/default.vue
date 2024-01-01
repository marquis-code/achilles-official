<template>
  <main>
    <Nuxt />
    <CursorFx color="#ffffff" color-hover="#f1c40f" />
  </main>
</template>

<script>
import { CursorFx } from "@luxdamore/vue-cursor-fx";
import "@luxdamore/vue-cursor-fx/dist/CursorFx.css";
export default {
  name: "default",
  components: { CursorFx }
};
</script>
