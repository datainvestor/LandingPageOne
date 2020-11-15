<template>
  <section class="stats">
    <v-slide-y-reverse-transition appear>
      <v-container :class="$vuetify.breakpoint.smAndDown && 'px-6'">
        <div
          class="stats-heading text-center"
        >Welcome to the best platform for building applications of all types with modern architecture and scaling</div>
        <v-row >
          <v-col cols="12" md="4" align-self="start">
            <div style="text-align: center;">
              <i class="fas fa-server fa-3x"></i>
              <h3>10,349,405</h3>
              <p class="text-secondary">Deployments</p>
            </div>
          </v-col>
          <v-col cols="12" md="4">
            <div style="text-align: center;">
              <i class="fas fa-upload fa-3x"></i>
              <h3>987 TB</h3>
              <p class="text-secondary">Published</p>
            </div>
          </v-col>
          <v-col cols="12" md="4">
            <div style="text-align: center;">
              <i class="fas fa-project-diagram fa-3x"></i>
              <h3>2,343,265</h3>
              <p class="text-secondary">Projects</p>
            </div>
          </v-col>
        </v-row>
      </v-container>
    </v-slide-y-reverse-transition>
  </section>
</template>

<script>
export default {};
</script>

<style scoped>
.stats {
  padding-top: 100px;
}

.stats-heading {
  max-width: 500px;
  margin: auto;
  font-size: 20px;
}

.stats h3 {
  font-size: 35px;
}

.stats p {
  font-size: 20px;
}

.text-secondary {
  color: #1c3fa8;
}
</style>