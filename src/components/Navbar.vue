<template>
  <header class="bg-white shadow h-16 flex justify-between items-stretch">
    <router-link :to="{name: 'home'}" class="inline-flex items-center h-full text-purple-500 font-bold text-[18px] px-5" >
      Home
    </router-link>

    <div class="flex items-center ">
      <router-link :to="{name: 'byName'}" class="inline-flex items-center transition-colors px-2 h-full hover:bg-purple-100">
        Search Meals
      </router-link>
      <router-link :to="{name: 'byLetter'}" class="inline-flex items-center transition-colors px-2 h-full hover:bg-purple-100">
        Meals By Letter
      </router-link>
      <router-link :to="{name: 'Ingredients'}" class="inline-flex items-center transition-colors px-1 h-full hover:bg-purple-100">
        Meals By Ingredients
      </router-link>
    </div>
  </header>
</template>