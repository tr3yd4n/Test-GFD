<script setup>
import TeamCard from './TeamCard.vue'

const users = [
  { name: 'Alice Johnson', image: 'https://placehold.co/130x173' },
  { name: 'Bob Smith', image: 'https://placehold.co/130x173' },
  { name: 'Claire Lee', image: 'https://placehold.co/130x173' },
  { name: 'David Brown', image: 'https://placehold.co/130x173' },
  { name: 'Ella Rose', image: 'https://placehold.co/130x173' },
]
</script>


<template>

  <!-- Our Story -->
  <section class="w-full bg-gray-100">

  <!-- Mobile and Desktop Layout Combined -->
  <div class="relative overflow-hidden">

    <!-- Mobile Layout -->
    <div class="w-100 h-[767px] relative bg-neutral-100 sm:hidden">
      <img class="w-[684px] h-[473px] left-[22px] top-[28px] absolute" src="https://placehold.co/684x473" />
      <img class="w-[274px] h-[155px] left-[132px] top-[10px] absolute border-[7px] border-white" src="https://placehold.co/260x141" />
      <div class="w-15 left-[47px] top-[78px] absolute justify-start text-black font-['Red_Hat_Display']">
        Bi-Fold Doors
      </div>
    </div>
  
  </div>
  </section>


  <!--Our Team Section -->
  <section class="p-8">
    <div class="w-full border-b border-black mb-6 ml-6">
      <h2 class="text-2xl font-bold pb-2">Our Team</h2>
    </div>
    
    <!--Buttons for Team Grid pagination-->
    <div class="flex gap-1 ml-6">
<button class="w-6 h-6 rounded-full bg-black flex items-center justify-center">
  <svg
    xmlns="http://www.w3.org/2000/svg"
    fill="white"
    viewBox="0 0 24 24"
    stroke-width="1.5"
    stroke="currentColor"
    class="w-4 h-4 rotate-180"
  >
    <path
      stroke-linecap="round"
      stroke-linejoin="round"
      d="m8.25 4.5 7.5 7.5-7.5 7.5"
    />
  </svg>
</button>

      <button class="w-6 h-6 rounded-full bg-black flex items-center justify-center">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          fill="white"
          viewBox="0 0 24 24"
          stroke-width="1.5"
          stroke="currentColor"
          class="w-4 h-4"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            d="m8.25 4.5 7.5 7.5-7.5 7.5"
          />
        </svg>
      </button>
    </div>


    <!--Team Grid (will make into a component when adding pagination controls)-->
    <div class="w-100 flex flex-wrap gap-1 p-4">
      <TeamCard
        v-for="user in users"
        :key="user.name"
        :name="user.name"
        :image="user.image"
      />
    </div>  
  </section>




</template>



<style scoped>
</style>
