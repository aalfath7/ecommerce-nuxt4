<template>
  <nav class="bg-white border border-gray-100 shadow-sm top-0 z-50">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="flex justify-between h-16 items-center">
        <!-- logo -->
        <div class="flex-shrink-0">
          <NuxtLink href="/" class="text-2xl font-bold text-orange-400"
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

        <!-- search and icons -->
        <div class="flex items-center space-x-4">
          <div class="hidden md:block">
            <input
              type="text"
              placeholder="Search Products"
              class="px-3 py-1 rounded-full border border-gray-300 focus:outline-none focus:ring-2 focus:ring-orange-400"
            />
          </div>
          <button class="text-gray-700 hover:text-orange-600 cursor-pointer">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              viewBox="0 0 24 24"
              stroke-width="1.5"
              stroke="currentColor"
              class="size-6"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                d="M2.25 3h1.386c.51 0 .955.343 1.087.835l.383 1.437M7.5 14.25a3 3 0 0 0-3 3h15.75m-12.75-3h11.218c1.121-2.3 2.1-4.684 2.924-7.138a60.114 60.114 0 0 0-16.536-1.84M7.5 14.25 5.106 5.272M6 20.25a.75.75 0 1 1-1.5 0 .75.75 0 0 1 1.5 0Zm12.75 0a.75.75 0 1 1-1.5 0 .75.75 0 0 1 1.5 0Z"
              />
            </svg>
          </button>
          <button class="text-gray-700 hover:text-orange-600 cursor-pointer">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              viewBox="0 0 24 24"
              stroke-width="1.5"
              stroke="currentColor"
              class="size-6"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                d="M15.75 6a3.75 3.75 0 1 1-7.5 0 3.75 3.75 0 0 1 7.5 0ZM4.501 20.118a7.5 7.5 0 0 1 14.998 0A17.933 17.933 0 0 1 12 21.75c-2.676 0-5.216-.584-7.499-1.632Z"
              />
            </svg>
          </button>
        </div>

        <!-- mobile menu -->
      </div>
    </div>
  </nav>
</template>
