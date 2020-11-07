<template>
    <v-app-bar
    id="core-toolbar"
    color="#047aed"
    flat
 :height="getHeight"
    app
  >
      <v-row  style="margin:0 auto; max-width:1100px;" align="center">
           <v-col class="pa-0 d-flex" :class="{'justify-center': $vuetify.breakpoint.smAndDown}" cols="12" md="9" >

          
    <v-toolbar-title class="display-1 px-0 align-center">
        <span>
          <span class="font-weight-thin" style="color:white;">Loruki.</span>
        </span>
    </v-toolbar-title>
</v-col>
<v-col  class="px-0 d-flex justify-center" cols="12" md="3">


<div class="navbar">
         <nav>
                <ul>
                    <li><a href="#">Home</a></li>
                    <li><a href="#">Features</a></li>
                    <li><a href="#">Docs</a></li>
                </ul>
            </nav>
</div>
</v-col>
      </v-row>
  </v-app-bar>
</template>

<script>
export default {
    computed:{
       getHeight(){
            return this.$vuetify.breakpoint.smAndDown ? 128 : 73;
          }
     }
}
</script>

<style scoped>
 .navbar a:hover {
  border-bottom: 2px #fff solid;
}
ul {
  list-style-type: none;
}
a {
  text-decoration: none;
  color: #333;
}
.navbar ul {
  display: flex;
}
.navbar a {
  color: #fff;
  padding: 10px;
  margin: 0 5px;
}
.navbar .flex {
  justify-content: space-between;
}

@media (max-width: 500px) {

  .navbar ul {
    padding: 10px;
    background-color: rgba(0, 0, 0, 0.1);
  }
}
</style>