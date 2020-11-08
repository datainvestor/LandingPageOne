<template>
 <section id="home">
   <showcase />
 </section>
</template>

<script>
  export default {
    name: 'Home',
    components: {
      Showcase: () => import('./Showcase'),

    },
  }
</script>

<style>

</style>