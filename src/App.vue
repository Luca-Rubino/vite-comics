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
@use'./styles/general.sass' as *;

*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
};
</style>