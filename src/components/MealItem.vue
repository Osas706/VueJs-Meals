<template>
  <div class="bg-white shadow rounded-xl">
    <router-link :to="{ name: 'mealDetails', params: { id: meal.idMeal } }">
      <img
        :src="meal.strMealThumb"
        :alt="meal.strMeal"
        class="rounded-t-xl w-full h-48 object-cover"
      />
    </router-link>

    <div class="p-3">
      <h3 class="font-bold mb-2">{{ meal.strMeal }}</h3>
      <p class="mb-2">Category: {{ meal.strCategory }}</p>
      <div class="flex items-center justify-between">
        <YoutubeBtn :href="meal.strYoutube"> Youtube </YoutubeBtn>
      </div>
    </div>
  </div>
</template>

<script setup>
import YoutubeBtn from "./YoutubeBtn.vue";

const { meal } = defineProps({
  meal: {
    required: true,
    type: Object,
  },
});

</script>
