<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <v-card>
    <v-layout>
      <v-app-bar color="primary" prominent>
        <v-toolbar-title>Learn Vue</v-toolbar-title>
      </v-app-bar>
      <div class="mt-16 flex flex-col gap-4 border-r p-4">
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </div>
      <v-main class="min-h-screen">
        <v-card-text>
          <RouterView />
        </v-card-text>
      </v-main>
    </v-layout>
  </v-card>



</template>