<script>
import { navLinks } from "../../constants/navLink";

export default {
  data() {
    return {
      navLinks: navLinks,
    };
  },
};
</script>

<template>
  <div class="sidebar w-[250px] min-h-screen bg-slate-800 relative ">
    <a
      href="#"
      class="logo text-center text-2xl p-3 block text-purple-300 font-bold"
      >DASHBOARD</a
    >

    <ul class="list">
      <li
        class="list_item p-4 shadow-2xl my-2 bg-purple-300 hover:bg-purple-500 duration-200"
        v-for="el in navLinks"
      >
        <a :href="el.link" class="list_item--link text-lg">
          <i :class="el.icon"></i> <span class="ms-3">{{ el.title }}</span>
        </a>
      </li>
    </ul>
  </div>
</template>

<style></style>
