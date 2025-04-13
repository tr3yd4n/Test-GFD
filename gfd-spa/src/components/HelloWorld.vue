<script setup>
import TeamCard from './TeamCard.vue'
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
    <div class="w-full border-b border-black mb-6">
      <h2 class="text-2xl font-bold pb-2">Our Team</h2>
    </div>
    <TeamCard name="Alice Johnson" image="https://placehold.co/130x174" />
  </section>




</template>



<style scoped>
</style>
