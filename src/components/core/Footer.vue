<template>
  <div id="footer">
    <v-footer class="white--text px-0 px-md-6 py-12" color="#002240" height="auto">
      <v-row style="margin:0 auto; max-width:1100px;" align="center">
        <v-col cols="12" md="4">
          <div>
            <h1>Loruki</h1>
            <p>Copyright &copy; 2020</p>
          </div>
        </v-col>

        <v-col cols="12" md="4" class="d-flex">
          <nav>
            <ul>
              <li>
                <router-link class="font-weight-light white--text" to="/index">Home</router-link>
              </li>
              <li>
                <router-link class="font-weight-light white--text" to="/about">Features</router-link>
              </li>
              <li>
                <router-link to="/docs" class="font-weight-light white--text">Docs</router-link>
              </li>
            </ul>
          </nav>
        </v-col>

        <v-col cols="12" md="4">
          <div class="social">
            <a href="#">
              <i class="fab fa-github fa-2x" style="color: white;"></i>
            </a>
            <a href="#">
              <i class="fab fa-facebook fa-2x" style="color: white;"></i>
            </a>
            <a href="#">
              <i class="fab fa-instagram fa-2x" style="color: white;"></i>
            </a>
            <a href="#">
              <i class="fab fa-twitter fa-2x" style="color: white;"></i>
            </a>
          </div>
        </v-col>
      </v-row>
    </v-footer>
  </div>
</template>

<script>
export default {
  name: "CoreFooter",

  data: () => ({
    socials: [
      { icon: "mdi-facebook-box", href: "#" },
      { icon: "mdi-twitter", href: "#" },
      { icon: "mdi-discord", href: "#" },
      { icon: "mdi-send", href: "#" },
      { icon: "mdi-reddit", href: "#" },
      { icon: "mdi-bitcoin", href: "#" },
      { icon: "mdi-youtube", href: "#" },
      { icon: "mdi-medium", href: "#" }
    ]
  })
};
</script>

<style lang="scss">
#footer {
  @media screen and (min-width: 960px) {
    margin-top: 200px;
  }
}

.social {
  a {
    margin: 0 10px;
  }
}
ul {
  list-style-type: none;
}
</style>
