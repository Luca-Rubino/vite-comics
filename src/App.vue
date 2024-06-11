<script>
import AppHeader from './components/AppHeader.vue';
import AppFooter from './components/AppFooter.vue';
export default {
  components: {
    AppHeader,
    AppFooter,
  }
}

</script>

<template>
    <AppHeader></AppHeader>
    <AppFooter></AppFooter>
</template>

<style lang="scss">
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body{
  font-family: "Roboto", sans-serif;
  font-weight: 500;
  font-style: normal;
}

li{
  list-style: none;
}

a {
  text-decoration: none;
  color: black;
}
</style>