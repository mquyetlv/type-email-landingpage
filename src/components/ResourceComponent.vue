<template>
  <div class="bg-second-color pt-36">
    <div>
      <div
        class="container-layout md:w-[840px] mx-auto max-w-full px-5 md:px-0"
      >
        <h1 class="text-intro text-center text-[52px] font-[600]">
          Online shoppers into loyal, lifetime customers with email & sms
          marketing
        </h1>
      </div>

      <div class="container-layout container mx-auto">
        <div class="flex flex-col md:flex-row gap-10 mt-16">
          <img
            class="w-full h-auto flex-1"
            src="../assets/images/photo-resource.png"
            alt=""
          />
          <div class="flex-1 px-4 py-7 flex items-center justify-center">
            <p class="text-[24px]">
              "New 2022, we sent a few email blasts with MailChimp here and
              there, but it wasn't a focus. Once we shiftedaway from retail-only
              sales to eCornmerce soles, driving customer awareness through
              email became a must-have, and our ESP wasn't cutting
            </p>
          </div>
        </div>
      </div>
    </div>

    <div class="mt-36">
      <div
        class="container-layout md:w-[840px] mx-auto max-w-full px-5 md:px-0"
      >
        <h1 class="text-intro text-center text-[52px] font-[600]">
          Sendlane Resource Library
        </h1>
        <div class="text-center flex justify-center">
          <p class="w-[330px] max-w-full text-[18px]">
            Cat in tuch with of our compare and take a personal tour of Sraklune
          </p>
        </div>

        <div class="mt-8 mb-20 flex gap-2 justify-center">
          <div class="btn-resource active">Articals</div>
          <div class="btn-resource">Ebooks</div>
          <div class="btn-resource">Products</div>
        </div>

        <div class="flex gap-6 flex-col md:flex-row">
          <template v-for="(card, index) in cardsResoure" :key="index">
            <CardResourceComponent :card="card" :isActive="index == 2" />
          </template>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import CardResourceComponent from './CardResourceComponent.vue';

const cardsResoure = [
  {
    image: require("../assets/images/girl-1.jpg"),
    title: "Email Marketing",
    descript: "Now to Grow lbw Email List 5 Email",
  },
  
  {
    image: require("../assets/images/girl-2.jpg"),
    title: "Real-time anylitics",
    descript: "Now to Grow lbw Email List 5 Email",
  },
  
  {
    image: require("../assets/images/girl-3.jpg"),
    title: "Marketing Autonation",
    descript: "Now to Grow lbw Email List 5 Email",
  },
];
</script>

<style scoped>
.btn-resource {
  display: inline-block;
  height: 50px;
  padding: 0 24px;
  display: flex;
  align-items: center;
  justify-content: center;
  border-radius: 12px;
  font-size: 20px;
}

.btn-resource.active {
  background: var(--primary-bg-color);
  color: #dfff1b;
}
</style>
