<template>
  <section class="w-full mt-6 lg:mt-48">
    <div class="max-w-8xl mx-auto flex flex-col gap-5 lg:pl-20">
      <div class="w-100% border-b border-black ml-6">
        
        <h2
          class="text-xl md:text-3xl lg:text-5xl font-bold pb-2"
          style="font-family: 'Red Hat Display', sans-serif"
        >
          Our Team
        </h2>
      </div>

      <!--Buttons for Team Grid pagination-->
      <div class="flex gap-1 ml-6 w-full justify-start lg:justify-end">
        <button
          class="w-6 h-6 lg:w-12 lg:h-12 rounded-full bg-gray-100 flex items-center justify-center transition-all duration-300"
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            viewBox="0 0 24 24"
            stroke-width="3.5"
            stroke="black"
            class="w-4 h-4 lg:w-6 lg:h-6 rotate-180"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              d="m8.25 4.5 7.5 7.5-7.5 7.5"
            />
          </svg>
        </button>

        <button
          class="w-6 h-6 lg:w-12 lg:h-12 lg:mr-6 rounded-full bg-gray-100 flex items-center justify-center transition-all duration-300"
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            viewBox="0 0 24 24"
            stroke-width="3.5"
            stroke="black"
            class="w-4 h-4 lg:w-6 lg:h-6"
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
      <div
        class="grid grid-cols-2 sm:grid-cols-4 lg:grid-cols-5 gap-6 ml-6 justify-between"
      >
        <TeamCard
          v-for="teamMember in teamMembers"
          :key="teamMember.name"
          :name="teamMember.name"
          :image="teamMember.image"
          :image2="teamMember.image2"
          :job-title="teamMember.jobTitle"
        />
      </div>

      <!-- buttons for pagination page count -->
      <div class="flex gap-2 ml-6">
        <div class="w-[10px] h-[10px] bg-black rounded-full"></div>
        <div class="w-[10px] h-[10px] bg-black rounded-full"></div>
        <div class="w-[10px] h-[10px] bg-black rounded-full"></div>
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
