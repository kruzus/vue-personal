<template>
  <Navbar />
</template>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Noto+Sans+JP&display=swap");
$backgroundColor: rgb(247, 247, 247);
body,
html {
  margin: 0;
  padding: 0;
  font-family: "Noto Sans JP", sans-serif;
  background: $backgroundColor;
}

*,
*::before,
*::after {
  box-sizing: border-box;
}
</style>
<script>
import Navbar from "./components/Navbar.vue";
export default {
  components: {
    Navbar,
  },
};
</script>
