<template>
  <section class="bg-amber-50">
    <div class="max-w-screen-xl mx-auto grid grid-cols-1 md:grid-cols-2">
      <div class="">
        <div class="py-24 space-y-5">
          <div
            class="inline-block text-sm tracking-widest px-2 py-1 bg-yellow-400 rounded-full"
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
            class="inline-block bg-black hover:bg-gray-700 text-white font-thin px-5 py-3 rounded-full"
            >Explore Deals</NuxtLink
          >
        </div>
      </div>
      <div class="flex justify-center items-center">
        <img
          class="w-1/2"
          src="/svg/order-confirmed-2-48.svg"
          alt="order confirmed ilustration"
        />
      </div>
    </div>
  </section>
</template>
