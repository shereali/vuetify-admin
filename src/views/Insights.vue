<template>
  <v-container>
    <v-layout row>
      <v-flex md3>
        <v-list>
          <v-header>
            <h2 class="pa-md-4">
              <strong>Insight</strong>
            </h2>
          </v-header>
          <v-subheader>Reporting On Jun 2020</v-subheader>
        </v-list>

        <v-list>
          <!-- <v-subheader>REPORTS</v-subheader> -->
          <v-list-item-group v-model="item" color="primary">
            <v-list-item v-for="(item, i) in items" :key="i">
              <v-list-item-icon>
                <v-icon v-text="item.icon"></v-icon>
              </v-list-item-icon>
              <v-list-item-content>
                <v-list-item-title v-text="item.text"></v-list-item-title>
              </v-list-item-content>
            </v-list-item>
          </v-list-item-group>
        </v-list>
        <v-spacer></v-spacer>
        <v-list>
          <v-header>
            <strong>Save Recommendatin</strong>
          </v-header>
          <v-list-item-group v-model="item" color="primary">
            <v-list-item v-for="(item, i) in items" :key="i">
              <v-list-item-icon>
                <v-icon v-text="item.icon"></v-icon>
              </v-list-item-icon>
              <v-list-item-content>
                <v-list-item-title v-text="item.text"></v-list-item-title>
              </v-list-item-content>
            </v-list-item>
          </v-list-item-group>
        </v-list>
      </v-flex>
      <v-flex md9>
        <v-layout row style="text-align:center;">
          <v-flex md4>
            <v-card class="pa-md-4 mx-lg-auto" color="white" width="250px">
              <h5 style="color:#528BFF;">Process</h5>
              <v-card-text>Adjust screen size to see spacing changes</v-card-text>
            </v-card>
          </v-flex>
          <v-flex md4>
            <v-card class="pa-md-4 mx-lg-auto" color="white" width="250px">
              <h5 style="color:#528BFF;">Governace</h5>
              <v-card-text>Adjust screen size to see spacing changes</v-card-text>
            </v-card>
          </v-flex>
          <v-flex md4>
            <v-card class="pa-md-4 mx-lg-auto" color="white" width="250px">
              <h5 style="color:#528BFF;">Communication</h5>
              <v-card-text>Adjust screen size to see spacing changes</v-card-text>
            </v-card>
          </v-flex>
        </v-layout>
        <v-layout row>
          <v-flex md12 class="mt-10">
            <v-card class="mx-lg-auto pa-md-4 pl-md-10" style="width:95%">
              <v-header>
                <h2>
                  <strong>Adjust screen size to see spacing changes</strong>
                </h2>
                <h5>Adjust screen size</h5>
              </v-header>
              <br />
              <v-header>
                <h4 style="color:#1D78D2;">Detail Explaination</h4>
                <p
                  class="pa-md-2"
                >Lorem ipsum dolor, sit amet consectetur adipisicing elit. Nemo quae consequuntur accusantium cumque corrupti dolor eius optio unde non excepturi? Mollitia sunt ipsa illo ea nesciunt a dolorem facilis atque!</p>
              </v-header>
              <v-header class="pa-md-4">
                <h4 class="pa-md-4">Insight Affect</h4>
                <p
                  class="pa-md-4"
                >Lorem ipsum dolor, sit amet consectetur adipisicing elit. Nemo quae consequuntur accusantium cumque corrupti dolor eius optio unde non excepturi? Mollitia sunt ipsa illo ea nesciunt a dolorem facilis atque!</p>
                <p
                  class="pa-md-4"
                >Lorem ipsum dolor, sit amet consectetur adipisicing elit. Nemo quae consequuntur accusantium cumque corrupti dolor eius optio unde non excepturi? Mollitia sunt ipsa illo ea nesciunt a dolorem facilis atque!</p>
              </v-header>
            </v-card>
          </v-flex>
          <v-flex md4></v-flex>
          <v-flex md8></v-flex>
        </v-layout>
      </v-flex>
    </v-layout>
  </v-container>
</template>
<script>
export default {
  data() {
    return {
      item: 1,
      items: [
        { text: "Progress", icon: "mdi-clock" },
        { text: "Governace", icon: "mdi-account" },
        { text: "Planning", icon: "mdi-flag" }
      ]
    };
  }
};
</script>
