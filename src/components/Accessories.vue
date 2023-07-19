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
          <ul class="flex justify-center">
            <li>
              <svg
                xmlns="http://www.w3.org/2000/svg"
                viewBox="0 0 24 24"
                fill="currentColor"
                class="mr-1 h-5 w-5 text-warning">
                <path
                  fill-rule="evenodd"
                  d="M10.788 3.21c.448-1.077 1.976-1.077 2.424 0l2.082 5.007 5.404.433c1.164.093 1.636 1.545.749 2.305l-4.117 3.527 1.257 5.273c.271 1.136-.964 2.033-1.96 1.425L12 18.354 7.373 21.18c-.996.608-2.231-.29-1.96-1.425l1.257-5.273-4.117-3.527c-.887-.76-.415-2.212.749-2.305l5.404-.433 2.082-5.006z"
                  clip-rule="evenodd" />
              </svg>
            </li>
            <li>
              <svg
                xmlns="http://www.w3.org/2000/svg"
                viewBox="0 0 24 24"
                fill="currentColor"
                class="mr-1 h-5 w-5 text-warning">
                <path
                  fill-rule="evenodd"
                  d="M10.788 3.21c.448-1.077 1.976-1.077 2.424 0l2.082 5.007 5.404.433c1.164.093 1.636 1.545.749 2.305l-4.117 3.527 1.257 5.273c.271 1.136-.964 2.033-1.96 1.425L12 18.354 7.373 21.18c-.996.608-2.231-.29-1.96-1.425l1.257-5.273-4.117-3.527c-.887-.76-.415-2.212.749-2.305l5.404-.433 2.082-5.006z"
                  clip-rule="evenodd" />
              </svg>
            </li>
            <li>
              <svg
                xmlns="http://www.w3.org/2000/svg"
                viewBox="0 0 24 24"
                fill="currentColor"
                class="mr-1 h-5 w-5 text-warning">
                <path
                  fill-rule="evenodd"
                  d="M10.788 3.21c.448-1.077 1.976-1.077 2.424 0l2.082 5.007 5.404.433c1.164.093 1.636 1.545.749 2.305l-4.117 3.527 1.257 5.273c.271 1.136-.964 2.033-1.96 1.425L12 18.354 7.373 21.18c-.996.608-2.231-.29-1.96-1.425l1.257-5.273-4.117-3.527c-.887-.76-.415-2.212.749-2.305l5.404-.433 2.082-5.006z"
                  clip-rule="evenodd" />
              </svg>
            </li>
            <li>
              <svg
                xmlns="http://www.w3.org/2000/svg"
                viewBox="0 0 24 24"
                fill="currentColor"
                class="mr-1 h-5 w-5 text-warning">
                <path
                  fill-rule="evenodd"
                  d="M10.788 3.21c.448-1.077 1.976-1.077 2.424 0l2.082 5.007 5.404.433c1.164.093 1.636 1.545.749 2.305l-4.117 3.527 1.257 5.273c.271 1.136-.964 2.033-1.96 1.425L12 18.354 7.373 21.18c-.996.608-2.231-.29-1.96-1.425l1.257-5.273-4.117-3.527c-.887-.76-.415-2.212.749-2.305l5.404-.433 2.082-5.006z"
                  clip-rule="evenodd" />
              </svg>
            </li>
          </ul>
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
