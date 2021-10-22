<template>
  <div id="app">
    <v-card>
      
    </v-card>

    <v-card>
      <v-text-field
        label="Email"
        :rules="rules"
      ></v-text-field>

      <v-card-title>Customer Experience</v-card-title>
      <v-divider></v-divider>
      <v-card-text>
        <v-radio-group
          v-model="customer"
          column
        >

          <v-radio
            label="John"
            value="john"
            color="red"
          ></v-radio>

          <v-radio
            label="James"
            value="james"
            color="blue"
          ></v-radio>

          <v-radio
            label="Kim"
            value="kim"
            color="white"
          ></v-radio>

        </v-radio-group>
      </v-card-text>
      
      <v-card-title>Wild Card</v-card-title>
      <v-divider></v-divider>
      <v-card-text>
        <v-radio-group
          v-model="wildcard"
          column
        >

          <v-radio
            label="Mary"
            value="mary"
            color="red"
          ></v-radio>

          <v-radio
            label="Queen"
            value="queen"
            color="blue"
          ></v-radio>

          <v-radio
            label="Aisha"
            value="aisha"
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
          Submit
        </v-btn>
      </v-card-actions>
    </v-card>
  </div>
</template>

<script>
export default {
  data() {
    return {
      customer: null,
      wildcard: null,
      rules: [value => !!value || 'Required.']
    }
  }
}
</script>
<style scoped>
</style>
