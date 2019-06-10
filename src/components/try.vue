<template>
  <v-container fluid grid-list-xl>
    <div class = "mainday">
    <v-layout wrap align-center>
      <v-flex xs12 sm6 d-flex>
        <v-select
          :items="items"
          label="Day"
        ></v-select>
      </v-flex>
    </v-layout>
    </div>
  </v-container>
</template>

<script>
  export default {
    data: () => ({
      items: ['Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday', 'Sunday']
    })
  }
</script>

<style>
.mainday{
  width: 500px;
  margin-left: 200px;
}
</style>
