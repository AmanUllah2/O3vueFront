<template>
  <v-app id="inspire">
    <div class="selectors">
    <v-container fluid grid-list-xl class="con">
      <v-layout wrap align-center>
        <v-flex xs3 sm3 d-flex>
          <v-select
            :items="item1"
            label="Day"
            solo
          ></v-select>
        </v-flex>
        <v-flex xs3 sm3 d-flex>
          <v-select
            :items="item2"
            label="Start Time"
            solo
          ></v-select>
        </v-flex>
        <p> To </p>
        <v-flex xs3 sm3 d-flex>
          <v-select
            :items="item3"
            label="End Time"
            solo
          ></v-select>
        </v-flex>
        <v-flex xs3 sm2 d-flex>
          <div class="add">
          <v-btn color="success">Add</v-btn>
          </div>
        </v-flex>
      </v-layout>
    </v-container>
    </div>
  </v-app>
</template>
  
<script>
export default {
  data: () => ({
    item1: ['Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday', 'Sunday'],
    item2: ['4:00 am', '5:00 am','6:00 am','7:00 am','8:00 am','9:00 am','10:00 am','11:00 am', '12:00 pm', '1:00 pm', '2:00 pm', '3:00 pm', '4:00 pm', '5:00 pm', '6:00 pm', '7:00 pm','8:00 pm','9:00 pm','10:00 pm'],
    item3: ['4:00 am', '5:00 am','6:00 am','7:00 am','8:00 am','9:00 am','10:00 am','11:00 am', '12:00 pm', '1:00 pm', '2:00 pm', '3:00 pm', '4:00 pm', '5:00 pm', '6:00 pm', '7:00 pm','8:00 pm','9:00 pm','10:00 pm'],

})
}
</script>

<style>
.con{
  height: 50px;
}

.add{
  margin-top: -25px;
  margin-left: 40px; 
}
</style>
