<template>
  <v-app>
    <v-app-bar
        app
        color="#9f0404"
        class="menu"
    >
      <div class="d-flex align-center">
        <a href="/" class="link-logo">
          <v-img
              alt="Vuetify Logo"
              class="shrink mr-2"
              contain
              src="./assets/embraseg.png"
              transition="scale-transition"
              width="140"
          />
        </a>


      </div>
      <v-app-bar-nav-icon
          @click="changeMenu"
          large
          class="icon-menu"

      ></v-app-bar-nav-icon>

      <v-spacer class="space"></v-spacer>

      <v-btn
          to="/"
          text
          class="link"
      >
        <span class="mr-2" style="color: white">Home</span>
        <!-- <v-icon>mdi-open-in-new</v-icon> -->
      </v-btn>
      <v-btn
          to="/products"
          text
          class="link"
      >
        <span class="mr-2" style="color: white">Produtos</span>
        <!-- <v-icon>mdi-open-in-new</v-icon> -->
      </v-btn>
      <v-btn
          to="/contact"
          text
          class="link"
      >
        <span class="mr-2" style="color: white">Contato</span>
        <!-- <v-icon>mdi-open-in-new</v-icon> -->
      </v-btn>
    </v-app-bar>
    <v-navigation-drawer v-model="drawer" absolute temporary>
      <v-list nav dense>
        <v-list-item-group>
          <v-list-item v-for="(item, index) in items" :key="index">
            <router-link
                :to="{ name: item }"
                style="text-decoration: none; color: darkred;"
                class="link-mobile"
            >
              <v-list-item-title
                  style="font-size: 1.6rem; margin-top: 28px;"
                  @click="tab = index"
              >{{ item }}</v-list-item-title
              >
            </router-link>
          </v-list-item>
        </v-list-item-group>
      </v-list>
    </v-navigation-drawer>

    <v-main>
      <router-view/>
    </v-main>
  </v-app>
</template>

<script>

export default {
  name: 'App',

  data: () => ({
    drawer: false,
    items: ["home", "products", "contact"],
  }),
  methods: {
    changeMenu() {
      this.drawer = true;
    },
  },
};
</script>
<style lang="scss" scoped>
.menu{
  .icon-menu {
    display: none;
  }
}
@media screen and (max-width: 450px) {
  .menu {
    .icon-menu {
      display: block;
      color:white;
    }
    .link-logo {
      display: none;
    }
    .space {
      display: none;
    }
    ::v-deep .v-navigation-drawer__content .v-list v-sheet .theme--light .v-list--dense .v-list--nav  {
      color: #9F0404;
      background-color: yellow;
      .link-mobile {
        font-size: 28pt;
        padding: 7%;
        width: 90%;
        border: 1px solid black;
        border-radius: 7px;
        text-align: center;
        color: #9F0404;
      }
    }

  }
}
</style>
