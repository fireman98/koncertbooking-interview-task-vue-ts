<script setup lang="ts">
import { RouterView } from 'vue-router'
</script>

<template>
  <div class="root__wrapper">
    <div class="root__sidebar"></div>
    <div class="root__content">
      <RouterView />
    </div>
  </div>
</template>

<style scoped lang="scss">
$sidebar-width: 250px;

.root {
  &__wrapper {
  }

  &__sidebar {
    position: fixed;
    top: 0;
    bottom: 0;
    left: 0;
    width: $sidebar-width;
    background-color: var(--intermediate_3);
  }

  &__content {
    position: relative;
    margin-left: $sidebar-width;
    padding: 0 50px 0 50px;
  }
}
</style>

<style lang="scss">
* {
  box-sizing: border-box;
  padding: 0;
  margin: 0;
}

body {
  --primary: #00adb3;
  --secondary: #819d9e;
  --danger: #b32557;
  --intermediate_3: #e2ecec;
}
</style>
