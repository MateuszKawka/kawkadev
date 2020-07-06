<template>
  <div>
    <Nuxt />
  </div>
</template>

<script>
import  Navigation  from "~/components/Navigation";
export default {
  components: {
    Navigation
  },
  data() {
    return {};
  }
};
</script>

<style lang="scss" >
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Roboto Slab';
}

.container {
  width: 100%;
  height: 100%;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  @include gradient-background;
  position: relative;
}

.section__title {
    width: 100%;
    text-align: center;
    margin: $s5 0;
}
</style>