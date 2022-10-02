<template>
  <div class="home">
    <Home
      msg="We provide the best strategy
to grow up your business"
    />
  </div>
</template>

<script>
// @ is an alias to /src
import Home from "@/components/Home.vue";

export default {
  name: "HomeView",
  components: {
    Home,
  },
};
</script>

<style scoped lang="scss">
.home {
  padding-top: 100px;
}
</style>
