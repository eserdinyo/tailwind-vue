<template>
  <div >
    <Header class="hidden md:flex" />
    <div class="flex">
      <Sidebar class="hidden md:flex" />
      <Main/>
    </div>
  </div>
</template>

<script>
import Header from "@/components/Header";
import Sidebar from "@/components/Sidebar";
import Main from "@/components/Main";
export default {
  components: {
    Header,
    Sidebar,
    Main
  }
};
</script>

