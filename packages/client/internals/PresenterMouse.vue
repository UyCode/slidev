<script setup lang="ts">
import { sharedState } from '../state/shared'
</script>

<template>
  <div
    v-if="sharedState.cursor"
    class="absolute top-0 left-0 right-0 bottom-0 pointer-events-none text-xl"
  >
    <ph:cursor-fill
      class="absolute"
      :style="{ left: `${sharedState.cursor.x}%`, top: `${sharedState.cursor.y}%` }"
    />
  </div>
</template>
