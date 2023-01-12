<!--
* @Component: 
* @Maintainer: J.K. Yang
* @Description: 
-->
<script setup lang="ts">
import { useCustomizeThemeStore } from "@/store/customizeTheme";
const customizeTheme = useCustomizeThemeStore();

// Page title
const title = ref("AdminPro NuxtJs Dashboard");

useHead({
  meta: [{ content: title }],
  titleTemplate: (titleChunk) => {
    return titleChunk
      ? `${titleChunk} - AdminPro NuxtJs Dashboard`
      : "AdminPro NuxtJs Dashboard";
  },
});
</script>
<template>
  <div>
    <v-app>
      <v-toolbar> </v-toolbar>
      <v-navigation-drawer> sss </v-navigation-drawer>
      <v-main>
        <slot />
      </v-main>
    </v-app>
  </div>
</template>

<style scoped lang="scss"></style>
