<template>
  <div class="content">
    <HeaderComponent />
    <router-view />
    <FooterComponent />
  </div>
</template>

<script>
import HeaderComponent from "./components/shared/Header.vue";
import FooterComponent from "./components/shared/Footer.vue";
export default {
  components: { HeaderComponent, FooterComponent },
};
</script>

