<template>
  <v-dialog
    v-model="dialog"
    :fullscreen="$vuetify.breakpoint.smAndDown"
    :hide-overlay="$vuetify.breakpoint.smAndDown"
    max-width="800"
    transition="dialog-bottom-transition"
  >
    <v-card>
      <v-toolbar
        color="white"
        flat
        :height="56"
      >
        <v-btn
          icon
          @click="dialog = false"
        >
          <v-icon>mdi-close</v-icon>
        </v-btn>
        <v-toolbar-title class="font-weight-bold">지역 선택</v-toolbar-title>
        <v-spacer></v-spacer>
      </v-toolbar>
      <v-card-text class="grey lighten-3 pa-4">
        <v-item-group>
          <v-container>
            <v-row dense>
              <v-col
                v-for="n in 3"
                :key="n"
                cols="12"
                md="4"
              >
                <v-item v-slot="{ active, toggle }">
                  <v-card
                    class="d-flex align-center"
                    flat
                    @click="toggle"
                  >
                    {{active}}
                    active
                  </v-card>
                </v-item>
              </v-col>
            </v-row>
          </v-container>
        </v-item-group>
      </v-card-text>
    </v-card>
  </v-dialog>
</template>

<script>
export default {
  data: () => ({
    dialog: false,
    notifications: false,
    sound: true,
    widgets: false,
  }),
  methods: {
    open () {
      this.dialog = true
    }
  }
}
</script>

<style>

</style>
