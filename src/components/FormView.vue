<template>
  <v-form>
    <v-container class="justify-center">
      <v-row>
        <v-col cols="6" sm="3">
          <Dropdown
            :options="[
              { id: 1, name: 'Option 1' },
              { id: 2, name: 'Option 2' },
              { id: 3, name: 'Option 3' },
            ]"
            v-on:selected="validateSelection"
            v-on:filter="getDropdownValues"
            :disabled="false"
            name="zipcode"
            :maxItem="10"
            placeholder="Please select an option"
            autocomplete="false"
          >
          </Dropdown>
        </v-col>
        <!-- <v-col cols="6" sm="3">
          <v-text-field
            v-model="title"
            :rules="rules"
            outlined
            counter="2"
            hint="This field uses counter prop"
            label="Repo Count"
          ></v-text-field>
        </v-col> -->
      </v-row>
    </v-container>
  </v-form>
</template>

<script>
import Dropdown from "vue-simple-search-dropdown";
export default {
  components: { Dropdown },
};
</script>