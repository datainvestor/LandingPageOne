<template>
 <section id="home">
   <showcase />
   <stats />
   <cli />
   <cloud />
 </section>
</template>

<script>
  export default {
    name: 'Home',
    components: {
      Showcase: () => import('./Showcase'),
      Stats: () => import('./Stats'),
      Cli: () => import('./Cli'),
      Cloud: () => import('./Cloud')
    },
  }
</script>

<style>

</style>