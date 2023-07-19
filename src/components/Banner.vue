<template>
  <div class="lg:flex md:flex w-full mb-10 relative">
    <div class="bg-[#36314C] w-11/12">
      <div
        class="bg-[#211C37] w-[600px] absolute h-[393px] rounded-3xl top-[22px] left-[44px]">
        <div
          class="bg-gradient-to-r from-[#6E3187] to-[#601E7C] flex justify-around items-center mx-auto mt-6 rounded-3xl w-[470px] h-[90px]">
          <div
            class="text-center bg-white w-[240px] p-2 rounded-xl font-Roboto bg-">
            <h1 class="font-Roboto font-medium text-xl text-[#211C37]">
              Rentals
            </h1>
            <p class="font-Roboto text-base">Daily | Weekly | Monthly</p>
            <div class="bg-white w-4 h-4 rotate-45 left-[190px] absolute"></div>
          </div>
          <div class="text-center text-white">
            <h1 class="font-Roboto font-medium text-2xl">Repair or Service</h1>
            <p class="font-Roboto text-sm">OnSite at your comfort</p>
          </div>
        </div>
        <h1
          class="text-center mt-4 text-white font-Roboto text-2xl font-medium">
          Cycle Rental in Mumbai
        </h1>
        <div class="bg-white mx-auto mt-6 rounded-3xl w-[470px] h-[100px]">
          <div class="flex items-center ml-7">
            <img
              src="https://i.ibb.co/jT1p5Fv/material-symbols-location-on-outline.png"
              alt=""
              class="w-8 h-8 mt-2" />
            <h1 class="font-Roboto font-medium mt-2 ml-6 text-black text-2xl">
              Delivery or Pickup Pincode
            </h1>
          </div>
          <hr class="mt-3 bg-[#867EA8] h-[2px]" />
          <div class="flex justify-around items-center mt-3">
            <div class="flex items-center gap-2 mb-2">
              <img src="https://i.ibb.co/G9nCyJw/uiw-date.png" alt="" />
              <h1 class="font-Roboto text-[#867EA8] text-xl font-medium">
                start Date
              </h1>
            </div>
            <div
              className="divider h-[46px] w-[1px] mt-[-12px] bg-[#867EA8] divider-horizontal"></div>
            <div class="flex items-center gap-2 mb-2">
              <img src="https://i.ibb.co/G9nCyJw/uiw-date.png" alt="" />
              <h2 class="font-Roboto text-[#867EA8] text-xl font-medium">
                End Date
              </h2>
            </div>
          </div>
        </div>
        <button
          class="w-[480px] ml-[60px] mt-[35px] font-Roboto text-white font-bold text-xl h-[50px] rounded-3xl bg-[#71AE0D]">
          Search Available Cycles
        </button>
      </div>
    </div>
    <div>
      <img
        src="https://i.ibb.co/TLTwGnH/e9c93f9149c15809dfd36dba76a76baf.jpg"
        alt="" />
      <div class="absolute font-Roboto top-[150px] right-[65px]">
        <h1 class="text-white font-medium text-3xl">
          Ride to your <br />
          <span class="font-medium text-5xl">Next Adventure</span>
        </h1>
        <div class="bg-[#211C37] mt-5 ml-5 font-Roboto w-80 h-36 round">
          <h1 class="text-lg p-2 text-[#F2AB3E] text-center">
            Get flat 20% off on your first <br />
            Rental. Use Code:
          </h1>
          <div
            class="bg-[#6D3187] ml-16 rounded-full flex items-center justify-center w-48 h-14 mb-4">
            <h1 class="text-white text-2xl font-extrabold">WELCOME20</h1>
          </div>
        </div>
      </div>
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
