<template>

    <v-card>
      <v-card-title>Select Team</v-card-title>
      <v-divider></v-divider>
      <v-card-text>
        <v-radio-group
          v-model="radiogroup"
          column
        >

          <v-radio
            label="ManU"
            value="manu"
            color="red"
          ></v-radio>

          <v-radio
            label="Chelsea"
            value="chelsea"
            color="blue"
          ></v-radio>

          <v-radio
            label="Arsenal"
            value="arsenal"
            color="white"
          ></v-radio>

        </v-radio-group>
      </v-card-text>
      <v-divider></v-divider>
      <v-card-actions>
        <v-btn
          color="blue darken-1"
          class="button"
          text
        >
          Vote
        </v-btn>
      </v-card-actions>
    </v-card>

</template>

<script>
export default {
  data() {
    return {
      radiogroup: null
    }
  }
}
</script>
<style scoped>
</style>
