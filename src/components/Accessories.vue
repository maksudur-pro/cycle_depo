<template>
  <div>
    <div class="flex items-center justify-between mt-10">
      <h1 class="text-[#36314C] ml-7 mb-5 text-3xl font-Roboto font-medium">
        Shop Accessories
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
            :alt="item.badge"
            class="p-6 w-[320px] h-[290px]" />
        </figure>
        <img
          src="https://i.ibb.co/nbJzb5Q/mdi-cards-heart-outline.png"
          alt=""
          class="w-6 h-6 absolute" />
        <p
          className="absolute -rotate-90 rounded-t-lg right-[-35px] top-8 mt-4 px-4 bg-slate-900 w-[100px] text-center text-white">
          {{ item.badge }}
        </p>
        <div class="flex justify-center items-center gap-2">
          <img :src="item.color[0].color2" alt="" />
          <img :src="item.color[0].color1" alt="" />
          <img :src="item.color[0].color3" alt="" />
        </div>
        <div className="card-body font-Roboto">
          <h2 className="text-center text-lg">{{ item.name }}</h2>
          <div
            className="card-actions justify-around mt-4 items-center font-Roboto">
            <h1 class="text-lg font-bold">{{ item.price }}</h1>
            <button
              className="bg-[#6D3186] text-white rounded-full font-bold w-[122px]  h-[41px]">
              View Details
            </button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import accessories from "../components/accessories.json";
export default {
  data() {
    return {
      data: accessories,
    };
  },
};
</script>
