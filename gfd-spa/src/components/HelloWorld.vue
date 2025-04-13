<script setup>
import TeamCard from "./TeamCard.vue";

const users = [
  {
    name: "Alice Johnson",
    image: "https://placehold.co/130x173",
    image2: "https://placehold.co/130x173",
    jobTitle: "Job Title",
  },
  {
    name: "Bob Smith",
    image2: "https://placehold.co/130x173",
    image: "https://placehold.co/130x173",
    jobTitle: "Job Title",
  },
  {
    name: "Claire Lee",
    image: "https://placehold.co/130x173",
    image2: "https://placehold.co/130x173",
    jobTitle: "Job Title",
  },
  {
    name: "David Brown",
    image: "https://placehold.co/130x173",
    image2: "https://placehold.co/130x173",
    jobTitle: "Job Title",
  },
  {
    name: "Ella Rose",
    image: "https://placehold.co/130x173",
    image2: "https://placehold.co/130x173",
    jobTitle: "Job Title",
  },
  {
    name: "Jack Jones",
    image: "https://placehold.co/130x173",
    image2: "https://placehold.co/130x173",
    jobTitle: "Job Title",
  },
];
</script>

<template>
  <!-- Our Story -->
  <section class="w-full bg-gray-100">
    <!-- Mobile and Desktop Layout Combined -->
    <div class="relative overflow-hidden">
      <!-- Mobile Layout -->
      <div class="w-100 h-[767px] relative bg-neutral-100 sm:hidden">
        <img
          class="w-[684px] h-[473px] left-[22px] top-[28px] absolute"
          src="https://placehold.co/684x473"
        />
        <img
          class="w-[274px] h-[155px] left-[132px] top-[10px] absolute border-[7px] border-white"
          src="https://placehold.co/260x141"
        />
        <div
          class="w-15 left-[47px] top-[78px] absolute justify-start text-black font-['Red_Hat_Display']"
        >
          Bi-Fold Doors
        </div>
      </div>
    </div>
  </section>

  <!--Company Value & Ethos-->
  <section class="w-full bg-gray-100 py-8">
    <div class="max-w-7xl mx-auto flex flex-col md:flex-row gap-6">
      <!-- Image Column -->
      <div class="w-full md:w-1/2">
        <!-- <h2 class="text-2xl font-bold pb-2">Company Values & Ethos</h2> -->
        <div class="relative w-full h-[98px]">
          <div
            class="bg-blue-100 w-[126px] h-[98px] absolute top-0 right-0 z-2"
          ></div>
          <h2
            class="text-[20px] font-bold absolute top-0 left-[35px] w-[153px] h-[52px]"
          >
            Company <br />Values & Ethos
          </h2>
        </div>
        <div class="relative w-full h-[260px] overflow-hidden">
          <img
            src="https://placehold.co/269x171"
            alt="Placeholder 1"
            class="absolute top-0 left-[114px] border-2 z-1"
          />
          <img
            src="https://placehold.co/214x155"
            alt="Placeholder 2"
            class="absolute top-[105px] left-[35px]"
          />
        </div>
      </div>

      <!-- Content Column -->
      <div class="w-full md:w-2/3 py-4">
        <div class="w-100% h-[153px] bg-red-500 mb-4 mr-6 lg:mr-0"></div>

        <div class="w-100% h-[173.8px] bg-blue-500 mb-4 ml-6 lg:ml-0"></div>

        <p
          class="p-8 bg-black text-sm md:text-base lg:text-lg text-white md:bg-transparent md:text-black mb-4"
        >
          We know that our continued success is down to our customers, and
          treating them with respect. Starting from humble beginnings means that
          we value each and every customer equally, regardless of the order
          size.
        </p>
        <p
          class="p-8 bg-black text-sm md:text-base lg:text-lg text-white md:bg-transparent md:text-black mb-4"
        >
          As the world becomes more automated by the day, we promise never to
          lose the personal touch with our customers that we built the
          foundations of the business on. Our staff are friendly, knowledgeable
          and always happy to assist.
        </p>
      </div>
    </div>
  </section>

  <!--Our Team Section -->
  <section class="py-4">
    <div class="w-100% border-b border-black mb-6 ml-6">
      <h2 class="text-2xl font-bold pb-2">Our Team</h2>
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
    <div class="w-100% flex flex-wrap justify-content-between gap-3 ml-6 mt-6">
      <TeamCard
        v-for="user in users"
        :key="user.name"
        :name="user.name"
        :image="user.image"
        :image2="user.image2"
        :job-title="user.jobTitle"
      />
    </div>
  </section>
</template>

<style scoped></style>
