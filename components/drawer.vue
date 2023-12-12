<template>
    <v-app>
      <v-container fluid>
        <!-- Your main content goes here -->
        <router-view></router-view>
      </v-container>
       <!-- Button to toggle the drawer -->
    <v-btn @click="toggleDrawer">Toggle Drawer</v-btn>
      <v-navigation-drawer :right="drawerRight" :bottom="drawerBottom"  v-model="drawerVisible">
        <!-- Your drawer content goes here -->
    
      </v-navigation-drawer>
    </v-app>
  </template>
  
  <script>
  export default {
    data() {
      return {
        drawerRight: true,
        drawerBottom: true,
      };
    },
    methods: {
      handleItemClick(item) {
        // Handle item click here
        console.log(`Clicked on ${item.text}`);
      },
      toggleDrawer() {
      // Toggle the visibility of the drawer
      this.drawerVisible = !this.drawerVisible;
    },
    },
  };
  </script>
  
  <style scoped>
  /* Add your custom styles here */
  </style>
  