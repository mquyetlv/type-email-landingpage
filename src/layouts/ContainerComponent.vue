<template>
  <div class="bg-primary-color pt-[80px] relative">
    <div class="intro md:w-[840px] max-w-full flex flex-col items-center mx-auto mt-[82px] mb-[76px]">
      <h1 class="text-intro text-center text-[52px] font-[600]">
        Online shoppers into loyal, lifetime customers with email & sms
        marketing
      </h1>

      <div class="mt-[46px] flex justify-center items-center">
        <button class="btn btn-large mr-[28px]">Getting started</button>
        <span class="text-[white] mr-[14px]">How it works</span>
        <img class="cursor-pointer" src="../assets/icons/icon-getting-started.svg" alt="">
      </div>
    </div>
      
    <div class="w-100 md:container mx-auto px-5">
      <img class="w-full h-auto" src="../assets/images/intro.png" alt="Intro image">
    </div>
  </div>
</template>

<script setup></script>
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
</style>
