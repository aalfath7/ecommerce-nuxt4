<template>
  <nav class="bg-white border border-gray-100 shadow-sm top-0 z-50">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="flex justify-between h-16 items-center">
        <!-- logo -->
        <div class="flex-shrink-0">
          <NuxtLink href="/" class="text-2xl font-bold text-orange-500"
            >ECommerce</NuxtLink
          >
        </div>

        <!-- desktop menu -->
        <div class="hidden md:flex space-x-5 items-center">
          <NuxtLink
            to="/"
            class="text-gray-700 hover:text-orange-600 text-medium"
            >Home</NuxtLink
          >
          <NuxtLink
            to="/"
            class="text-gray-700 hover:text-orange-600 text-medium"
            >Product</NuxtLink
          >
          <NuxtLink
            to="/"
            class="text-gray-700 hover:text-orange-600 text-medium"
            >Promo</NuxtLink
          >
          <NuxtLink
            to="/"
            class="text-gray-700 hover:text-orange-600 text-medium"
            >Contact</NuxtLink
          >
        </div>

        <div class="flex space-x-4">
          <!-- search and icons -->
          <div class="flex items-center space-x-4">
            <div class="hidden md:block">
              <input
                type="text"
                placeholder="Search Products"
                class="px-3 py-1 rounded-full border border-gray-300 focus:outline-none focus:ring-2 focus:ring-orange-400"
              />
            </div>
            <button>
              <IconCart />
            </button>
            <button>
              <IconUser />
            </button>
          </div>

          <!-- mobile menu button-->
          <div class="flex items-center md:hidden">
            <button @click="toggleMenu">
              <IconBar />
            </button>
          </div>
        </div>
      </div>

      <div v-if="isOpen" class="md:hidden p-4">
        <NuxtLink
          to="/"
          class="block py-2 text-gray-700 hover:text-orange-600 cursor-pointer"
          >Home</NuxtLink
        >
        <NuxtLink
          to="/"
          class="block py-2 text-gray-700 hover:text-orange-600 cursor-pointer"
          >Product</NuxtLink
        >
        <NuxtLink
          to="/"
          class="block py-2 text-gray-700 hover:text-orange-600 cursor-pointer"
          >Promo</NuxtLink
        >
        <NuxtLink
          to="/"
          class="block py-2 text-gray-700 hover:text-orange-600 cursor-pointer"
          >Contact</NuxtLink
        >
        <input
          type="text"
          placeholder="Search Product..."
          class="my-2 px-3 py-1 rounded-full border border-gray-300 focus:outline-none focus:ring-2 focus:ring-orange-600"
        />
      </div>
    </div>
  </nav>
</template>

<script setup lang="ts">
import IconCart from "~/components/icons/IconCart.vue";
import IconUser from "~/components/icons/IconUser.vue";
import IconBar from "~/components/icons/IconBar.vue";

const isOpen = ref(false);

const toggleMenu = () => {
  isOpen.value = !isOpen.value;
};
</script>
