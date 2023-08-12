<template>
  <div class="bg-primary-color pt-[80px] relative">
    <div
      class="intro container-layout md:w-[840px] max-w-full flex flex-col items-center mx-auto mt-[82px] mb-[76px]"
    >
      <h1 class="text-intro text-center text-[52px] font-[600]">
        Online shoppers into loyal, lifetime customers with email & sms
        marketing
      </h1>

      <div class="mt-[46px] flex justify-center items-center">
        <button class="btn btn-large mr-[28px]">Getting started</button>
        <span class="text-[white] mr-[14px] hidden sm:block">How it works</span>
        <img
          class="cursor-pointer"
          src="../assets/icons/icon-getting-started.svg"
          alt=""
        />
      </div>
    </div>

    <div class="intro container-layout w-100 md:container mx-auto px-5">
      <img
        class="w-full h-auto"
        src="../assets/images/intro.png"
        alt="Intro image"
      />
    </div>

    <div class="bg-third-color mt-[140px]">
      <div
        class="container-layout w-100 md:container mx-auto columns-1 md:columns-3"
      >
        <template v-for="(statis, index) in statistical" :key="index">
          <div class="card">
            <h1 class="text-[42px] font-[600]">{{ statis.value }}</h1>
            <p>{{ statis.title }}</p>
          </div>
        </template>
      </div>
    </div>
  </div>
</template>

<script setup>
const statistical = [
  { value: "1,700+", title: "Companies using Sendlance" },
  { value: "40 milion+", title: "Emails sent daily" },
  { value: "20,000+", title: "Users on sendlance" },
];
</script>

<style scoped>
.text-intro {
  background: var(
    --primary-color-lenier,
    linear-gradient(142deg, #e6ff4b 0%, #00bd82 100%)
  );
  background-clip: text;
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}

.card {
  padding: 66px 0 46px 0;
  text-align: center;
  color: var(--primary-bg-color);
}
</style>
