<script setup lang="ts">
import { themeChange } from 'theme-change';
import { onMounted } from 'vue';
import TxDialog from './components/TxDialog.vue';
import { Analytics } from '@vercel/analytics/react';

onMounted(() => {
  themeChange(false);
});
</script>

<template>
  <div>
    <RouterView />
    <TxDialog />
  </div>
</template>
