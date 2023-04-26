<script>
export default {
  name: "Header",
  props: {
    toggle: Function,
  },
};
</script>

<template>
  <header>
    <nav class="bg-slate-800 ">
      <a
        href="#"
        class="logo text-center text-2xl p-4 items-center text-purple-300 flex font-bold"
        >DASHBOARD</a
      >
      <div class="flex">
        <button
          @click="toggle"
          class="bg-blue-500 focus:ring-2 flex justify-center text-3xl absolute right-2 top-4 w-[36px] h-[36px] rounded-lg items-center  "
        >
          <i class="bx bx-menu"></i>
        </button>
      </div>
    </nav>
  </header>
</template>

<style></style>
