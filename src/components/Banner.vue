<template>
  <div class="lg:flex md:flex w-full mb-10 relative">
    <div class="bg-[#36314C] w-11/12">
      <div
        class="bg-[#211C37] w-[600px] absolute h-[393px] rounded-3xl top-[22px] left-[44px]">
        <div class="bg-white mx-auto mt-6 rounded-3xl w-[470px] h-[90px]"></div>
        <h1
          class="text-center mt-4 text-white font-Roboto text-2xl font-medium">
          Cycle Rental in Mumbai
        </h1>
        <div class="bg-white mx-auto mt-6 rounded-3xl w-[470px] h-[100px]">
          <div class="flex items-center ml-6">
            <img
              src="https://i.ibb.co/jT1p5Fv/material-symbols-location-on-outline.png"
              alt=""
              class="w-8 h-8" />
            <h1 class="font-Roboto font-medium text-black text-2xl">
              Delivery or Pickup Pincode
            </h1>
          </div>
        </div>
        <button
          class="w-[480px] ml-[60px] mt-[35px] font-Roboto text-white font-bold text-xl h-[50px] rounded-3xl bg-[#71AE0D]">
          Search Available Cycles
        </button>
      </div>
    </div>
    <div class="">
      <img
        src="https://i.ibb.co/TLTwGnH/e9c93f9149c15809dfd36dba76a76baf.jpg"
        alt=""
        class="" />
    </div>
  </div>
</template>

<script setup>
import { ref } from "vue";

const startDate = ref(""); // Use a ref to track the start date
const endDate = ref(""); // Use a ref to track the end date

const updateStartDate = (event) => {
  startDate.value = event.target.value; // Update the start date value
};

const updateEndDate = (event) => {
  endDate.value = event.target.value; // Update the end date value
};
</script>
