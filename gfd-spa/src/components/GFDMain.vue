<script setup>
import OurTeamSection from "./OurTeamSection.vue";
import CompanyValuesSection from "./CompanyValuesSection.vue";
import OurStorySection from "./OurStorySection.vue";

const users = [
  {
    name: "Tia Surname",
    image: "/images/Frame 220660.jpg",
    image2: "/images/IMG_9829.jpg",
    jobTitle: "Job Title",
  },
  {
    name: "Bob Smith",
    image: "/images/Frame 220660.jpg",
    image2: "/images/IMG_9829.jpg",
    jobTitle: "Job Title",
  },
  {
    name: "Claire Lee",
    image: "/images/Frame 220660.jpg",
    image2: "/images/IMG_9829.jpg",
    jobTitle: "Job Title",
  },
  {
    name: "David Brown",
    image: "/images/Frame 220660.jpg",
    image2: "/images/IMG_9829.jpg",
    jobTitle: "Job Title",
  },
  {
    name: "Ella Rose",
    image: "/images/Frame 220660.jpg",
    image2: "/images/IMG_9829.jpg",
    jobTitle: "Job Title",
  },
  {
    name: "Jack Jones",
    image: "/images/Frame 220660.jpg",
    image2: "/images/IMG_9829.jpg",
    jobTitle: "Job Title",
  },
];
</script>

<template>  
<div class="w-full overflow-hidden">
 <!-- Our Story -->
  <OurStorySection />

  <!--Company Values & Ethos-->
  <CompanyValuesSection />

  <!--Our Team Section -->
  <OurTeamSection />

</div>
 

  

</template>

<style scoped></style>
