<template>
  <section class="w-full mt-6">
    <div class="max-w-7xl mx-auto flex flex-col gap-6">
      <div class="w-100% border-b border-black ml-6">
        <h2 class="text-xl md:text-3xl lg:text-5xl font-bold pb-2">Our Team</h2>
      </div>

      <!--Buttons for Team Grid pagination-->
      <div class="flex gap-1 ml-6">
        <button
          class="w-6 h-6 rounded-full bg-black flex items-center justify-center"
        >
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

        <button
          class="w-6 h-6 rounded-full bg-black flex items-center justify-center"
        >
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
      <div class="w-100% flex flex-wrap justify-content-between gap-3 ml-6">
        <TeamCard
          v-for="teamMember in teamMembers"
          :key="teamMember.name"
          :name="teamMember.name"
          :image="teamMember.image"
          :image2="teamMember.image2"
          :job-title="teamMember.jobTitle"
        />
      </div>
    </div>


  </section>
</template>

<script setup>
import TeamCard from "./TeamCard.vue";

const teamMembers = [
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
