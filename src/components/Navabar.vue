<template>
  <v-navigation-drawer
    v-model="drawer"
    :mini-variant="mini"
    permanent
    :color="color"
    :expand-on-hover="expandOnHover"
    :src="bg"
    absolute
    dark
  >
    <v-list-item class="px-2">
      <v-list-item-avatar>
        <v-img src="https://randomuser.me/api/portraits/men/85.jpg"></v-img>
      </v-list-item-avatar>

      <v-list-item-title>John Leider</v-list-item-title>

      <v-btn icon @click.stop="mini = !mini">
        <v-icon>mdi-chevron-left</v-icon>
      </v-btn>
    </v-list-item>

    <v-divider></v-divider>

    <v-list class dense>
      <v-list-item to="/" link>
        <v-list-item-icon>
          <v-icon>mdi-home</v-icon>
        </v-list-item-icon>

        <v-list-item-content>
          <v-list-item-title>Home</v-list-item-title>
        </v-list-item-content>
      </v-list-item>
    </v-list>
    <v-list class dense>
      <v-list-item to="/insights" link>
        <v-list-item-icon>
          <v-icon>mdi-star</v-icon>
        </v-list-item-icon>

        <v-list-item-content>
          <v-list-item-title>Insights</v-list-item-title>
        </v-list-item-content>
      </v-list-item>
    </v-list>
    <v-list class dense>
      <v-list-item to="/monitoring" link>
        <v-list-item-icon>
          <v-icon>mdi-eye</v-icon>
        </v-list-item-icon>

        <v-list-item-content>
          <v-list-item-title>Monitoring</v-list-item-title>
        </v-list-item-content>
      </v-list-item>
    </v-list>
    <v-list class dense>
      <v-list-item to="/recommendation" link>
        <v-list-item-icon>
          <v-icon>mdi-pen</v-icon>
        </v-list-item-icon>

        <v-list-item-content>
          <v-list-item-title>Recommendation</v-list-item-title>
        </v-list-item-content>
      </v-list-item>
    </v-list>
    <v-list class dense>
      <v-list-item @click="mini = !mini" link>
        <v-list-item-icon>
          <v-icon>mdi-logout</v-icon>
        </v-list-item-icon>

        <v-list-item-content>
          <v-list-item-title></v-list-item-title>
        </v-list-item-content>
      </v-list-item>
    </v-list>
  </v-navigation-drawer>
</template>

<script>
export default {
  data() {
    return {
      drawer: true,
      items: [
        { title: "Home", icon: "mdi-home-city" },
        { title: "Monitoring", icon: "mdi-account" },
        { title: "Insights", icon: "mdi-account-group-outline" }
      ],
      mini: true,
      color: "primary",
      colors: ["primary", "blue", "success", "red", "teal", "white"],
      miniVariant: false,
      expandOnHover: false,
      background: true
    };
  },
  methods: {}
};
</script>