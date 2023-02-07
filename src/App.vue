<template>
  <TheHeader />
  <main>
    <Main />
  </main>
  <TheFooter />
</template>

<script>
import Main from "./views/Main";
import TheHeader from "./components/TheHeader";
import TheFooter from "./components/TheFooter";
export default {
  name: "App",
  components: {
    Main,
    TheHeader,
    TheFooter,
  },
};
</script>
