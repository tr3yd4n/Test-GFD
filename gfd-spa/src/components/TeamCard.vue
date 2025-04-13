<template>
  <div class="w-64 p-4 bg-white shadow-md rounded-lg flex flex-col items-center">
    <img
      :src="image"
      :alt="name"
      class="w-32 h-32 object-cover mb-4"
    />
    <!--<h3 class="text-lg font-semibold text-gray-800">{{ name }}</h3>-->
  </div>
</template>

<script setup>
defineProps({
  name: String,
  image: String,
})
</script>