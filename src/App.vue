<template>
  <v-layout class="rounded rounded-md">
    <v-app-bar :elevation="2">
      <template v-slot:prepend>
        <v-app-bar-nav-icon> </v-app-bar-nav-icon>
      </template>

    <v-app-bar-title>Menu</v-app-bar-title>
    </v-app-bar>
    <v-navigation-drawer>
      <v-list-item link to="/" title="INICIO"></v-list-item>
      <v-list-item link to="/imagen" title="JOKES Y IMAGENES"></v-list-item>
      <v-list-item link to="/tabla" title="DATOS"></v-list-item>
    </v-navigation-drawer>

    <v-main
      class="d-flex align-center justify-center"
      style="min-height: 300px"
    >
    <router-view></router-view>
    </v-main>
  </v-layout>
</template>
