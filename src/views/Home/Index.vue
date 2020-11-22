<template>
 <section id="home">
   <showcase />
   <stats />
   <cli />
   <cloud />
   <languages />
 </section>
</template>

<script>
  export default {
    name: 'Home',
    components: {
      Showcase: () => import('./Showcase'),
      Stats: () => import('./Stats'),
      Cli: () => import('./Cli'),
      Cloud: () => import('./Cloud'),
      Languages: () => import('./Languages')
    },
  }
</script>

<style>

</style>