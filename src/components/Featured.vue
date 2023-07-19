<template>
  <div>
    <div class="flex items-center justify-between">
      <h1 class="text-[#36314C] ml-7 mb-5 text-3xl font-Roboto font-medium">
        Featured Cycles
      </h1>
      <div class="flex items-center">
        <h1 class="mr-6 font-Roboto">View Full Catalogue</h1>
        <div class="flex items-center">
          <img src="https://i.ibb.co/NmhFHBB/Component-3.png" alt="" />
        </div>
      </div>
    </div>
    <div class="lg:flex md:flex gap-4">
      <div
        v-for="item in data"
        :key="item.id"
        className="card w-96 bg-base-100 font-Roboto shadow-xl">
        <figure>
          <img
            :src="item.image"
            :alt="item.brand"
            class="p-6 w-[340px] h-[260px]" />
        </figure>
        <p
          v-if="item.available"
          class="absolute text-sm font-Roboto p-4 text-[#FF4A49]">
          {{ item.available }}
        </p>
        <p
          className="absolute -rotate-90 rounded-t-lg right-[-28px] top-8 mt-4 px-4 bg-slate-900 w-[80px] text-center text-white">
          {{ item.badge }}
        </p>
        <div className="card-body p-0 pb-4 font-Roboto">
          <h2 className="text-center text-xl font-bold">{{ item.name }}</h2>
          <div class="flex items-center justify-around">
            <div class="flex items-center gap-2 text-[#999797]">
              <img
                src="https://i.ibb.co/GdWrSNC/bi-calendar-date.png"
                class="w-3 h-3"
                alt="" />
              <p class="text-sm">14+ Yrs</p>
            </div>
            <div class="flex items-center gap-2 text-[#999797]">
              <img
                src="https://i.ibb.co/m51gH24/mdi-human-male-height-variant.png"
                class="w-3 h-3"
                alt="" />
              <p class="text-sm">5'4"-6'</p>
            </div>
            <div class="flex items-center gap-2 text-[#999797]">
              <img
                src="https://i.ibb.co/vdBCTVx/fluent-emoji-high-contrast-wheel.png"
                class="w-3 h-3"
                alt="" />
              <p class="text-sm">27.5"/69cm</p>
            </div>
          </div>
          <div
            className="card-actions justify-around mt-4 items-center font-Roboto">
            <h1 class="text-sm font-bold">
              <span class="text-xl font-extrabold">{{ item.price }}</span>
              Monthly
            </h1>

            <button
              v-if="item.status === 'Book'"
              className="bg-[#6D3186] text-white rounded-full font-bold w-[122px]  h-[41px]">
              Book
            </button>
            <button
              v-else
              className="bg-[#827F90] text-white rounded-full font-bold w-[122px]  h-[41px]">
              PRE BOOK
            </button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import cycleData from "../components/cycleData.json";
export default {
  data() {
    return {
      data: cycleData,
    };
  },
};
</script>
