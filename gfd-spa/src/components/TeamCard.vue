<template>
  <div
    class="relative group w-[130px] h-[174px] overflow-hidden"
  >
    <!-- Job Title (Top Reveal) -->
    <p
      class="absolute top-0 left-0 w-full h-[10%] bg-white text-xs text-center italic font-semibold text-gray-800 translate-y-[-100%] opacity-0 group-hover:translate-y-0 group-hover:opacity-100 transition-all duration-500 ease-in-out z-10"
    >
      {{ jobTitle }}
    </p>

    <!-- Main Image (Default) -->
    <img
      :src="image"
      :alt="name"
      class="w-full h-full object-cover absolute top-0 left-0 transition-opacity duration-500 group-hover:opacity-0"
    />

    <!-- Hover Image (image2) -->
    <img
      :src="image2"
      :alt="`${name} hover image`"
      class="w-full h-full object-cover absolute top-0 left-0 opacity-0 transition-opacity duration-500 group-hover:opacity-100"
    />

    <!-- Router Link (Bottom Reveal) -->
    <RouterLink
      :to="'/user-card'"
      class="absolute bottom-0 left-0 w-full h-[10%] bg-white text-xs text-center font-medium text-gray-800 translate-y-full opacity-0 group-hover:translate-y-0 group-hover:opacity-100 transition-all duration-500 ease-in-out z-10 cursor-pointer"
    >
      View Profile
    </RouterLink>
  </div>
</template>

<script setup>
defineProps({
  name: String,
  image: String,
  image2: String,
  jobTitle: String,
})
</script>
