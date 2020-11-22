<template>
  <section class="languages">
    <v-container>
      <h2 class="lead mt-3 mb-4">Supported Languages</h2>
      <v-row>
        <v-col>
          <v-card shaped class="elevation-5">
            <h4 class="h4new pt-3" style="text-align: center;">Node.js</h4>
            <div class="py-3">
                <v-img max-height="80" contain src="../../assets/logos/node.png" />
            </div>
          </v-card>
        </v-col>
        <v-col>
          <v-card shaped class="elevation-5"> 
            <h4 class="h4new pt-3" style="text-align: center;">Python</h4>
            <div class="py-3">
            <v-img max-height="80" contain src="../../assets/logos/python.png" alt />
            </div>
            </v-card>
        </v-col>
        <v-col>
          <v-card shaped class="elevation-5">
            <h4  class="h4new pt-3" style="text-align: center;">C#</h4>
            <div class="py-3">
            <v-img max-height="80" contain src="../../assets/logos/csharp.png" alt />
            </div>
          </v-card>
        </v-col>
        <v-col>
          <v-card shaped class="elevation-5">
            <h4  class="h4new pt-3" style="text-align: center;">Ruby</h4>
            <div class="py-3">
            <v-img max-height="80" contain src="../../assets/logos/ruby.png" alt />
            </div>
          </v-card>
        </v-col>
        <v-col>
          <v-card shaped class="elevation-5">
            <h4 class="h4new pt-3" style="text-align: center;">PHP</h4>
            <div class="py-3">
            <v-img max-height="80" class="" contain src="../../assets/logos/php.png" alt />
            </div>
          </v-card>
        </v-col>
        <v-col>
          <v-card shaped class="elevation-5">
            <h4 class="h4new pt-3" style="text-align: center;">Scala</h4>
            <div class="py-3">
            <v-img max-height="80" contain src="../../assets/logos/scala.png" alt />
            </div>
          </v-card>
        </v-col>
        <v-col>
          <v-card shaped class="cc elevation-5">
            <h4 class="h4new pt-3" style="text-align: center;">Clojure</h4>
            <div class="py-3">
            <v-img max-height="80" contain src="../../assets/logos/clojure.png" alt />
            </div>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </section>
</template>

<script>
export default {};
</script>

<style scoped>
.lead {
  text-align: center;
  color: gray;
  font-size: 30px;
  font-weight: 300;
}

.h4new {
   color: gray;
  font-size: 20px;
  font-weight: 400;
}

.v-card {
  transition: transform .2s ease-in-out;
}

.v-card:hover {
  transform: translateY(-15px);
}

</style>