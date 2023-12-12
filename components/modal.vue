<template>
    <v-app>
      <v-container fluid>
        <!-- Your main content goes here -->
        <v-btn @click="openModal">Open</v-btn>
  
        <v-dialog v-model="modalVisible" max-width="600">
          <v-card>
            <v-card-title>
              <span class="headline">Modal Title</span>
              <v-icon icon="md:home"></v-icon>
            </v-card-title>
            <v-card-text>
              <!-- Your modal content goes here -->
              <p>This is the content of the modal.</p>
            </v-card-text>
            <v-card-actions>
              <v-btn color="primary" @click="closeModal">Close</v-btn>
            </v-card-actions>
          </v-card>
        </v-dialog>
      </v-container>
    </v-app>
  </template>
  
  <script>
  export default {
    data() {
      return {
        modalVisible: true,
      };
    },
    methods: {
      openModal() {
        this.modalVisible = true;
      },
      closeModal() {
        this.modalVisible = false;
      },
    },
  };
  </script>
  
  <style scoped>
  /* Add your custom styles here */
  </style>
  