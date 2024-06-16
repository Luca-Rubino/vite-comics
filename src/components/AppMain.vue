<script>
import Comics from '../components/Comics.vue';


export default {
        components: {
            Comics,
        },

    data() {
        return {

        }
    },
}

</script>

<template>

    <main>
        <section class="content">

            <p>-->Content goes here<--</p>
            
        </section>

        <Comics/>
    </main>

</template>

<style lang="scss" scoped>
@use '../../styles/general.scss' as *;
@use '../../styles/partials/variable.sass' as *;
@use '../../styles/partials/mixin.sass' as *;

section.content {
  background-color: black;
  color: white;
  padding: 3rem 13rem;
  font-size: 1.5rem;
  width: 100%;
}
</style>