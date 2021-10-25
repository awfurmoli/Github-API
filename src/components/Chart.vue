<template>
  <v-container>
    <v-row class="text-center">
      <v-col class="mb-4">
        <h1 class="display-2 font-weight-bold mb-3">
          {{ msg }}
        </h1>
        <button @click="getData">Get Data</button>
        <p class="subheading font-weight-regular">
          GitHub API, building a small web service that returns the top N
          repositories by star count for a specific language.
        </p>
      </v-col>
      <v-col class="mb-5" cols="12">
        <h2 class="headline font-weight-bold mb-3">The {{ language }} Repos</h2>

        <v-container class="justify-center">
          <v-row> <form-view></form-view> </v-row>
          <v-row>
            <h2>The Chart</h2>
            <the-chart></the-chart>
          </v-row>
        </v-container>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
import axios from "axios";
import TheChart from "./TheChart.vue";
import FormView from "./FormView.vue";

export default {
  components: { TheChart, FormView },
  data: () => ({
    name: "Chart",
    language: "Lang",
    records: [],
  }),
  props: {
    msg: String,
  },
  methods: {
    async getData() {
      const response = await axios.get("https://reqres.in/api/users?page=2");
      const result = await response.data.data;
      console.log(result);
      this.records = result;
    },
  },
  created() {
    this.getData();
  },
};
</script>

<!-- Add "scoped" to style this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
