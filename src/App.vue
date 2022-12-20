<template>
  <appHeader />
  <main>
    <appMain />
  </main>
  <appFooter />
</template>

<script>
import appHeader from "./components/Header";
import appMain from "./views/Main";
import appFooter from "./components/Footer";
export default {
  name: "App",
  components: {
    appHeader,
    appMain,
    appFooter,
  },
};
</script>
