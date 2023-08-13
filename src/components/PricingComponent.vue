<template>
  <div class="bg-second-color pt-36">
    <div class="container-layout md:w-[840px] mx-auto max-w-full px-5 md:px-0">
      <h1 class="text-intro text-center text-[52px] font-[600]">
        Online shoppers into loyal, lifetime customers with email & sms
        marketing
      </h1>
      <p class="text-center text-[16px]">
        Awareness through email be came a must-have, and our ESP wasn't cutting
      </p>
    </div>

    <div
      class="container container-layout mx-auto pt-24 flex flex-col-reverse md:flex-row gap-x-8"
    >
      <div class="break-after-column flex-1 px-5 md:px-0 mt-4 md:mt-0">
        <h2 class="text-[40px] font-[600]">
          Drive 30-40% of your revenue with email marekiting
        </h2>
        <p class="text-[18px] pt-4">
          Unlock customer insights to grow your business faster. Store all your
          customer data collected from storefront to marketing channels in one
          central hub far easy use in every strategy.
        </p>

        <div class="flex flex-col sm:flex-row pt-9 gap-x-3">
          <template
            v-for="(item, index) in modelsContentMarketing"
            :key="index"
          >
            <div class="flex-1 flex flex-col">
              <img
                :src="item.iconLink"
                alt="icon-home"
                class="w-[62px] h-auto"
              />
              <h1 class="pt-4 text-[20px] font-[600]">{{ item.header }}</h1>
              <p class="pt-1 text-[16px] mb-7">{{ item.descript }}</p>
              <a
                class="icon-read-more inline-block mt-auto relative cursor-pointer"
                >Read More</a
              >
            </div>
          </template>
        </div>
      </div>

      <div class="flex items-center justify-center flex-1">
        <img src="../assets/images/image-marketing.png" class="w-full h-auto" />
      </div>
    </div>

    <div
      class="container container-layout mx-auto pt-24 flex flex-col md:flex-row gap-x-8"
    >
      <div class="flex items-center justify-center flex-1">
        <img src="../assets/images/image-customer.png" class="w-full h-auto" />
      </div>

      <div class="break-after-column flex-1 px-5 md:px-0 mt-4 md:mt-0">
        <h2 class="text-[40px] font-[600]">
          Create raving fans that keep buying over and over you get the point.
        </h2>

        <p class="text-[18px] pt-4">
          Unlock customer insights to grow your business faster. Store all your
          customer data collected from storefront to marketing channels in one
          central hub far easy use in every strategy.
        </p>

        <span class="block text-[16px] text-[#1e1e1e] font-[600] mt-7">
          Our open rate has tripled and our click rate on links is up at least
          15%.
        </span>

        <button class="btn btn-large mt-12">Learn More</button>
      </div>
    </div>

    <div class="container-layout container mt-36 mx-auto">
      <h1 class="text-[50px] font-[600] text-center mb-14">Our some service</h1>
      <div class="flex gap-3 flex-col md:flex-row px-5 md:px-0">
        <template v-for="(item, index) in someServices" :key="index">
          <div class="card-item flex-1 pt-9 pb-16 px-11 rounded-[2px]">
            <div
              class="wrap-icon bg-fourth-color w-[66px] h-[66px] rounded-full flex items-center justify-center mb-11"
            >
              <img :src="item.iconLink" alt="" />
            </div>
            <h1 class="mb-4 text-[20px] font-[600]">{{ item.header }}</h1>
            <p>{{ item.content }}</p>
          </div>
        </template>
      </div>
    </div>

    <div class="bg-primary-color mt-36 py-16">
      <div class="container-layout container mt-36 mx-auto flex flex-col md:flex-row gap-16 px-5 md:px-0">
        <div class="text-[#fff] flex-1">
          <h1 class="text-[50px] font-[600] mb-1">Join forces with your favorite business tools</h1>
          <p class="text-[16px] mb-11">
            awareness through email became a must-have, and our ESP wasn't
            cutting
          </p>
          <button class="btn btn-small">
            <span class="block mr-2">See imagradtions</span>
            <img src="../assets/icons/arrow.svg" alt="">
          </button>
        </div>

        <div class="flex-1">
          <img src="../assets/images/images-service.png" class="w-full h-auto" alt="">
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
const modelsContentMarketing = [
  {
    iconLink: require("../assets/icons/icon-home.svg"),
    header: "Marketing Automation",
    descript:
      "From open rates to conversion performance, get access to tons of data.",
  },
  {
    iconLink: require("../assets/icons/icon-python.svg"),
    header: "Experiments",
    descript: "From sign up to sale track your contacts every move.",
  },
];

const someServices = [
  {
    iconLink: require("../assets/icons/letter.svg"),
    header: "Email Marketing",
    content:
      "Set up standing order in-app, and send money to any other bank account instantly",
  },
  {
    iconLink: require("../assets/icons/chat.svg"),
    header: "SMS Marketing",
    content:
      "Manage your account from your phone or computer. Do everything you need from the app.",
  },
  {
    iconLink: require("../assets/icons/cream.svg"),
    header: "Intellegent pop ups",
    content:
      "Your bank account lets you easily lock your card in the app, and later reorder it witha tap of a button",
  },
];
</script>

<style scoped>
.icon-read-more:hover::before {
  content: "";
  display: block;
  height: 2px;
  background: var(--primary-color);
  position: absolute;
  left: 0;
  width: 100px;
  bottom: 0;
}

.card-item:hover {
  cursor: pointer;
  background: #fdf9f1;
}

.card-item:hover .wrap-icon {
  background: var(--primary-color);
}
</style>
