<template>
  <section class="w-full mt-32 md:h-[730px]">
    <div class="max-w-7xl mx-auto flex flex-col md:flex-row gap-6">
      <!-- Image Column -->
      <div class="w-full md:w-1/2">
        <!-- <h2 class="text-2xl font-bold pb-2">Company Values & Ethos</h2> -->
        <div class="relative w-full h-[98px]">
          <div
            class="bg-gray-100 w-[126px] h-[98px] absolute top-0 right-0 md:hidden"
          ></div>
          <div
            class="bg-gray-100 w-full h-[101px] absolute top-[167px] left-0 md:hidden shadow-md shadow-gray-400"
          ></div>
          <h2
            class="text-xl md:text-3xl lg:text-5xl font-bold absolute top-0 left-[35px] h-[52px]"
            style="font-family: 'Red Hat Display', sans-serif"
          >
            Company <br />Values & Ethos
          </h2>
        </div>
        <div
          class="relative w-full h-[260px] md:h-full overflow-hidden lg:mt-10 flex justify-center items-center"
        >
          <img
            src="/images/_dsf2305_52920521840_o 2.jpg"
            alt="Placeholder 1"
            class="absolute top-0 left-[114px] z-10 w-[269px] h-[171px] object-cover shadow-md pr-8 mr-4"
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
          <img
            src="/images/DSI_Solid_Core_Thatched Cottage V1_170731 1.jpg"
            alt="Placeholder 2"
            class="absolute top-[50px] left-[450px] w-[170px] h-[235px] object-cover md:hidden"
          />
        </div>
      </div>

      <!-- Content Column -->
      <div class="w-full md:w-2/3">
        <!-- <div class="w-100% h-[153px] bg-red-500 mb-8 lg:mb-9 mr-6 lg:mr-0"></div> -->
        <div class="overflow-hidden w-full mb-8 lg:mb-10 ml-9 lg:ml-0">
          <div class="flex flex-nowrap gap-0">
            <img
              v-for="(img, index) in exampleImages"
              :key="index"
              :src="img"
              alt="Group image"
              class="h-[112px] md:h-[128px] lg:h-[153px] object-cover flex-shrink-0 p-0 m-0"
            />
          </div>
        </div>
        <p
          class="p-8 ml-2 mb-8 bg-black text-sm md:text-base lg:text-lg text-white md:bg-transparent md:text-black md:mb-1 md:p-2 md:hidden"
          style="font-family: 'Red Hat Display', sans-serif"
        >
          We know that our continued success is down to our customers, and
          treating them with respect. Starting from humble beginnings means that
          we value each and every customer equally, regardless of the order
          size.
        </p>

        <div
          class="w-100% h-[173.8px] bg-blue-500 mb-8 lg:mb-10 ml-9 lg:ml-0"
        ></div>

        <p
          class="p-8 ml-2 mb-8 bg-black text-sm md:text-base lg:text-lg text-white md:bg-transparent md:text-black md:mb-1 md:p-2 md:hidden"
          style="font-family: 'Red Hat Display', sans-serif"
        >
          As the world becomes more automated by the day, we promise never to
          lose the personal touch with our customers that we built the
          foundations of the business on. Our staff are friendly, knowledgeable
          and always happy to assist.
        </p>

        <p
          class="hidden font-semibold md:block pt-12 lg:text-base bg-transparent text-black h-[221px] lg:pb-[70px]"
          style="font-family: 'Red Hat Display', sans-serif"
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
        <hr class="w-full border-t border-black mt-6" />
      </div>
    </div>
  </section>
</template>

<script setup>
const exampleImages = [
  "/images/exampleGroupA/RectangleA.jpg",
  "/images/exampleGroupA/RectangleB.jpg",
  "/images/exampleGroupA/RectangleC.jpg",
  "/images/exampleGroupA/RectangleD.jpg",
  "/images/exampleGroupA/RectangleE.jpg",
];
</script>
