<template>
  <section class="cloud bg-blue my-2">
    <v-container :class="$vuetify.breakpoint.smAndDown && 'pt-0'">
      <v-row style="margin: 0 auto" align="center">

        <v-col cols="12" md="7" class="py-auto mx-auto">
          <div class="text-center">
            <div class="lg">Extreme Cloud Hosting</div>
            <p class="lead my-1">Cloud hosting like you've never seen. Fast, efficient and scalable</p>
            <v-btn to="/features" color="#002240" class="white--text">Read more</v-btn>
          </div>
        </v-col>

        <v-col cols="12" md="5" class="py-auto mx-auto">
          <v-img src="../../assets/cloud.png"></v-img>
        </v-col>
      </v-row>
    </v-container>
  </section>
</template>

<script>
export default {};
</script>

<style scoped>
.bg-blue {
  background: #047aed;
}
.lg {
  font-size: 3rem;
  color: white;
  font-weight: 300;
}

.lead {
  color: white;
  font-size: 20px;
  font-weight: 200;
}
</style>