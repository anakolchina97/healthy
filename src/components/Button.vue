<script setup lang="ts">
defineProps<{ text: string; className: string }>();
</script>

<template>
  <button class="button" :class="className">{{ text }}</button>
</template>

<style scoped lang="scss">
.button {
  border: none;
  outline: none;
  color: var(--color-primary);
  background: var(--color-green);
  font-family: "HelveticaNeueCondensed", Arial, Helvetica, sans-serif;
  &._big {
    padding: rem(25) rem(58);
    border-radius: rem(43);
    font-weight: 700;
    font-size: rem(18);
    line-height: 1.375rem;
    text-align: center;
    letter-spacing: 0.2em;
  }
  &._black {
    background: var(--color-primary);
  }
}
</style>
