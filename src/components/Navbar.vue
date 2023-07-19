<script setup>
import { RouterLink } from "vue-router";
</script>

<template>
  <div
    class="bg-[#36314C] hidden lg:block md:block text-white w-[378px] h-[30px] text-center rounded-b-2xl mx-auto">
    <h1 class="font-Roboto text-white font-medium text-sm">
      24/7 Customer query
      <span class="text-base font-black"> +91-8169026971</span>
    </h1>
  </div>
  <div class="navbar bg-base-100">
    <div class="navbar-start">
      <div class="dropdown">
        <label tabIndex="{0}" class="btn btn-ghost lg:hidden">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="h-5 w-5"
            fill="none"
            viewBox="0 0 24 24"
            stroke="currentColor">
            <path
              strokeLinecap="round"
              strokeLinejoin="round"
              strokeWidth="2"
              d="M4 6h16M4 12h8m-8 6h16" />
          </svg>
        </label>
        <ul
          tabIndex="{0}"
          class="menu menu-sm dropdown-content mt-3 z-[1] p-2 shadow bg-base-100 rounded-box w-52">
          <li>
            <RouterLink to="/">How it works</RouterLink>
          </li>
          <li>
            <RouterLink to="/blog">Blog</RouterLink>
          </li>
          <li>
            <RouterLink to="/">Events</RouterLink>
          </li>
          <li>
            <RouterLink to="/" class="fontstyle"> Rentals </RouterLink>
          </li>
          <li>
            <RouterLink to="/" class="fontstyle">
              Repairing Service
            </RouterLink>
          </li>
          <li>
            <RouterLink to="/" class="fontstyle"> Buy Accessories </RouterLink>
          </li>
          <li>
            <RouterLink to="/login" class="text-[#211C37] font-medium">
              Login or Sign Up</RouterLink
            >
          </li>
        </ul>
      </div>
      <img
        src="https://i.ibb.co/k3FWfvK/cycle-logo.jpg"
        class="w-[200px] h-[68px] mb-4 hidden lg:block md:block"
        alt="" />
    </div>
    <div class="navbar-center hidden lg:flex">
      <ul class="menu menu-horizontal px-1">
        <li>
          <RouterLink to="/" class="mt-1">How it works</RouterLink>
        </li>
        <li>
          <RouterLink to="/blog" class="mt-1">Blog</RouterLink>
        </li>
        <li>
          <RouterLink to="/" class="mt-1">Events</RouterLink>
        </li>
        <li>
          <RouterLink to="/" class="fontstyle"> Rentals </RouterLink>
        </li>
        <li>
          <RouterLink to="/" class="fontstyle"> Repairing Service </RouterLink>
        </li>
        <li>
          <RouterLink to="/" class="fontstyle"> Buy Accessories </RouterLink>
        </li>
        <li>
          <h1
            class="bg-[#FF4A49] rounded-3xl font-Roboto text-xl font-bold text-white">
            Become Partner
          </h1>
        </li>
      </ul>
    </div>
    <div class="navbar-end gap-4 items-center">
      <img
        src="https://i.ibb.co/WsjPL8c/material-symbols-login.jpg"
        class="hidden lg:block md:block"
        alt="" />
      <RouterLink
        to="/login"
        class="text-[#211C37] font-medium hidden lg:block md:block">
        Login or Sign Up</RouterLink
      >
    </div>
  </div>
</template>
