<template>
  <div class="w-[130px] h-[174]">
    
    <!--<p class="italic font-semibold text-gray-800 hidden">{{ job title }}</h3>-->
    <img
      :src="image"
      :alt="name"
      class="w-[130px] h-[174px] object-cover"
    />
    <RouterLink
    :to="'/user-card'"
    class="w-64 p-4 bg-white shadow-md rounded-lg hover:shadow-lg transition-shadow duration-300 hidden"
    >
        View Profile
    </RouterLink>

  </div>
</template>

<script setup>
defineProps({
  name: String,
  image: String,
})
</script>