<template>
<section class="showcase">
  <v-container
    class="px-0"
    :class="$vuetify.breakpoint.smAndDown && 'pt-0'"
  >
    <v-responsive class="overflow-visible" min-height="50vh">
      <v-row align="center" align-content="center" class="fill-height mx-0" justify="center">
        <v-slide-x-transition appear>
          <v-col align-self="start" cols="12" md="6">
            <div class="showcase-text white--text pt-6">
              <div class="text-h4 font-weight-light mt-12 mb-6">Easier Deployment</div>
              <p class="font-weight-thin" >Deploy web apps of all kinds, from large scale enterprise APIs to static websites for individuals. Fill out the form to try a demo of our platform</p>
                  <v-btn outlined color="white" class="font-weight-light">
                    Read More
                    </v-btn>
            </div>
          </v-col>
        </v-slide-x-transition>

        <v-slide-x-reverse-transition appear>
          <v-col cols="auto" class="form-card">
              <v-card class="rounded-card">
                  <v-card-title class="px-10 mb-6 pt-6 font-weight-light">
                      Request a Demo
                  </v-card-title>
             
            <v-form class="px-10 pb-4" ref="form" v-model="valid" lazy-validation>
              <v-text-field v-model="name" :counter="10" :rules="nameRules" label="Name" required></v-text-field>

              <v-text-field v-model="company" :counter="10" :rules="nameRules" label="Company" required></v-text-field>

              <v-text-field v-model="email" :rules="emailRules" label="E-mail" required></v-text-field>

              <v-btn color="#047aed" class="white--text mr-4" @click="validate">Send</v-btn>
            </v-form>
             </v-card>
          </v-col>
        </v-slide-x-reverse-transition>

      </v-row>
    </v-responsive>
  </v-container>
  </section>
</template>

<script>
export default {};
</script>

<style scoped>
.rounded-card{
    border-radius:20px;
}
.form-card {
    max-width: 400px;
    width: 100%;
    z-index: 100;
    margin-top:40px;
}

.showcase {
    background-color: #047aed;
    height: 400px;
    position:relative;
}

.showcase::before,
.showcase::after {
  content: '';
  position: absolute;
  height: 100px;
  bottom: -70px;
  right: 0;
  left: 0;
  background: #fff;
  transform: skewY(-3deg);
  -webkit-transform: skewY(-3deg);
  -moz-transform: skewY(-3deg);
  -ms-transform: skewY(-3deg);
}

@media (max-width: 768px) {
 .showcase-text {
    text-align: center;
    padding: 0;
  }
    .showcase {
    height: auto;
  }

  .form-card {
    max-width: 300px;
    width: 100%;
    z-index: 100;
    margin:auto;
    position:relative;
    top:60px;
}
}
</style>