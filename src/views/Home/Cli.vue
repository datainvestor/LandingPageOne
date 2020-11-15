<template>
  <section class="cli">
    <div class="container grid">
      <v-img src="../../assets/cli.png"></v-img>
      <v-card class="ma-2 pa-5 elevation-6">
        <h3>Easy to use, cross platform CLI</h3>
      </v-card>
      <v-card class="ma-2 pa-5 elevation-6">
        <h3>Deploy in seconds</h3>
      </v-card>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style scoped>
.container {
  max-width: 1100px;
  margin: 0 auto;
  overflow: auto;
  padding: 0 40px;
}

.grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 20px;
  justify-content: center;
  align-items: center;
  height: 100%;
}

.cli .grid {
  grid-template-columns: repeat(3, 1fr);
  grid-template-rows: repeat(2, 1fr);
}

.cli .grid > *:first-child {
  grid-column: 1 / span 2;
  grid-row: 1 / span 2;
}


@media screen and (max-width: 768px) {
  .grid {
    grid-template-columns: 1fr !important;
    grid-template-rows: 1fr !important;
  }
  .cli .grid > *:first-child {
    grid-column: 1 !important;
    grid-row: 1 !important;
  }
}
</style>