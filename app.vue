<template>
  <v-app>
    <v-main>
      <v-container>
        <v-text-field label="Message" v-model="message"></v-text-field>
      </v-container>
    </v-main>
  </v-app>

</template>


<script>
export default {
  name: 'App',
  data: () => ({
    message: '',
  }),
};
</script>
