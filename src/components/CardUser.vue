<template>
  <v-container>
    <v-row class="text-center">
      <v-card class="mx-auto my-12" width="376" rounded="md">
        <v-toolbar
          prominent
          height="125"
          src="https://cdn.vuetifyjs.com/images/cards/cooking.png"
          class="mb-4"
        >
          <template v-slot:extension>
            <v-row justify="center" class="my-auto mx-auto">
              <v-sheet
                color="white"
                elevation="0"
                height="64"
                rounded="pill"
                width="100%"
              >
                <v-row no-gutters>
                  <v-col cols="2">
                    <v-avatar left size="64">
                      <v-img src="https://cdn.vuetifyjs.com/images/john.png" />
                    </v-avatar>
                  </v-col>
                  <v-col>
                    <v-list-item-content class="text-left ml-4 pa-0">
                      <v-list-item-title>
                        <span class="text-h6 text--primary ma-0 pa-0">
                          valoracion: 4.5
                        </span>
                      </v-list-item-title>
                      <v-list-item-subtitle>
                        <span class="text-h6 text--primary">
                          valoracion: 4.5
                        </span>
                      </v-list-item-subtitle>
                    </v-list-item-content>
                  </v-col>
                </v-row>
              </v-sheet>
            </v-row>
          </template>
        </v-toolbar>

        <v-card-title>Netflix Premium</v-card-title>

        <v-card-text class="text-left">
          <p class="text-h6 text--primary">
            Lorem ipsum dolor sit amet.
          </p>
          <p class="text-h6 text--primary">
            Lorem ipsum dolor sit.
          </p>
          <div class="d-flex justify-space-between">
            <p class="text-h6 text--primary">
              valoracion: 4.5
            </p>
            <v-rating
              :value="4.5"
              color="amber"
              dense
              half-increments
              readonly
            ></v-rating>
          </div>
        </v-card-text>

        <v-card-actions class="grey lighten-3">
          <v-btn text block color="grey"
            >info de acceso guardadas <v-spacer></v-spacer>
            <v-icon left large>mdi-key</v-icon></v-btn
          >
        </v-card-actions>
      </v-card>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: "CardUser",

  data: () => ({
    loading: false,
    selection: 1
  }),

  methods: {
    reserve() {
      this.loading = true;

      setTimeout(() => (this.loading = false), 2000);
    }
  }
};
</script>
