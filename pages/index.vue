<template>
  <section class="p-4 md:p-20 bg-amber-50 shadow space-y-5">
    <div
      class="inline-block text-sm font-thin px-3 py-2 bg-yellow-400 rounded-full"
    >
      WELCOME DISCOUNT
    </div>

    <h1 class="text-5xl font-bold">
      BEST DEALS <br />
      ENDLESS DEALS
    </h1>

    <p>
      Discover the best deals across endless options,<br />
      offering quality and unbeatable variety daily.
    </p>

    <NuxtLink
      to="/"
      class="inline-block bg-black text-white font-thin px-5 py-3 rounded-full"
      >Explore Deals</NuxtLink
    >
  </section>
</template>

<script setup lang="ts">
definePageMeta({
  layout: "home",
});
</script>
