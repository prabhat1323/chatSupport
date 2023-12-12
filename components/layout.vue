<template>
    <v-app class="position-right-bottom with-box">
      <!-- Header -->
      <v-app-bar app>
        <v-toolbar-title>My App</v-toolbar-title>
      </v-app-bar>
  
      <!-- Main content area -->
      <v-main>
        <slot></slot>
      </v-main>
  
      <!-- Footer -->
      <v-footer app>
        <span>&copy; 2023 My App</span>
      </v-footer>

    </v-app>
  </template>
  