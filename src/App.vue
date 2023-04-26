<script>
import Sidebar from "./components/Sidebar/Sidebar.vue";
import Header from "./components/Header/Header.vue";
import Home from "./views/Home/Home.vue";
export default {
  data() {
    return {
      toggle: true,
    };
  },
  components: {
    Sidebar,
    Header,
    Home,
  },
  methods: {
    toggleMenu() {
      this.toggle = !this.toggle;
    },
  },
};
</script>

<template>
  <Header :toggle="toggleMenu"/>
  <main class="flex">
    <aside v-if="toggle" class="top-0 bg-white">
      <Sidebar />
    </aside>

    <section class="main top-0 ">
      <Home />
    </section>
  </main>
</template>

<style></style>
