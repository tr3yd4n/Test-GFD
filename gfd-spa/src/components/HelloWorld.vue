<script setup>
import TeamCard from "./TeamCard.vue";

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
  <!-- Our Story -->
  <section class="w-full bg-gray-100">
    <!-- Mobile and Desktop Layout Combined -->
    <div class="relative overflow-hidden">
      <!-- Mobile Layout -->
      <div class="w-100 h-[767px] relative bg-neutral-100">
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
  <section class="w-full mt-12">
    <div class="max-w-7xl mx-auto flex flex-col md:flex-row gap-6">
      <!-- Image Column -->
      <div class="w-full md:w-1/2">
        <!-- <h2 class="text-2xl font-bold pb-2">Company Values & Ethos</h2> -->
        <div class="relative w-full h-[98px]">
          <div
            class="bg-gray-100 w-[126px] h-[98px] absolute top-0 right-0 md:hidden"
          ></div>
          <h2
            class="text-xl md:text-3xl lg:text-5xl font-bold absolute top-0 left-[35px] h-[52px]"
          >
            Company <br />Values & Ethos
          </h2>
        </div>
        <div class="relative w-full h-[260px] md:h-full overflow-hidden">
          <img
            src="/images/_dsf2305_52920521840_o 2.jpg"
            alt="Placeholder 1"
            class="absolute top-0 left-[114px] z-10 w-[269px] h-[171px] object-cover shadow-md"
          />
          <img
            src="/images/_dsf2246_52920591768_o.jpg"
            alt="Placeholder 2"
            class="absolute top-[105px] left-[35px] w-[214px] h-[155px] object-cover"
          />
          <img
            src="/images/DSI_Solid_Core_Thatched Cottage V1_170731 1.jpg"
            alt="Placeholder 2"
            class="absolute top-[317px] left-[257px] w-[170px] h-[235px] object-cover hidden md:block"
          />
        </div>
      </div>

      <!-- Content Column -->
      <div class="w-full md:w-2/3 py-4">
        <div class="w-100% h-[153px] bg-red-500 mb-8 mr-6 lg:mr-0"></div>

        <p
          class="p-8 mb-8 bg-black text-sm md:text-base lg:text-lg text-white md:bg-transparent md:text-black md:mb-1 md:p-2 md:hidden"
        >
          We know that our continued success is down to our customers, and
          treating them with respect. Starting from humble beginnings means that
          we value each and every customer equally, regardless of the order
          size.
        </p>

        <div class="w-100% h-[173.8px] bg-blue-500 mb-8 ml-6 lg:ml-0"></div>

        <p
          class="p-8 mb-8 bg-black text-sm md:text-base lg:text-lg text-white md:bg-transparent md:text-black md:mb-1 md:p-2 md:hidden"
        >
          As the world becomes more automated by the day, we promise never to
          lose the personal touch with our customers that we built the
          foundations of the business on. Our staff are friendly, knowledgeable
          and always happy to assist.
        </p>
        <p
          class="hidden md:block pt-12 text-base lg:text-lg bg-transparent text-black"
        >
          We know that our continued success is down to our customers, and
          treating them with respect. Starting from humble beginnings means that
          we value each and every customer equally, regardless of the order
          size.
          <br />
          <br />
          As the world becomes more automated by the day, we promise never to
          lose the personal touch with our customers that we built the
          foundations of the business on. Our staff are friendly, knowledgeable
          and always happy to assist.
        </p>
      </div>
    </div>
  </section>

  <!--Our Team Section -->

  <section class="w-full mt-12">
    <div class="max-w-7xl mx-auto flex flex-col gap-6">
      <div class="w-100% border-b border-black mb-4 ml-6">
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
          v-for="user in users"
          :key="user.name"
          :name="user.name"
          :image="user.image"
          :image2="user.image2"
          :job-title="user.jobTitle"
        />
      </div>
    </div>
  </section>
</template>

<style scoped></style>
