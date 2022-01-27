<template>
  <div class="container">
    <breadcrumbs/>
    <MainHeader title="Floresta Macabra" />
    <Nuxt />
  </div>
</template>

<script>
import Breadcrumbs from '~/src/components/Breadcrumbs.vue';
import MainHeader from "../src/components/MainHeader.vue";

export default {
  components: {
    MainHeader,
    Breadcrumbs,
  },
};
</script>


<style scoped>
.container {
  max-width:1280px;
  margin:0 auto;
}
header {
  padding:0.7rem;
  margin-left: auto;
  margin-right: auto;
  background: black;
  background-size: cover;
  background-repeat: no-repeat;
  overflow: hidden;
  text-align: center;
  color: white;
}
</style>
