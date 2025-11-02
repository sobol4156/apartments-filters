<template>
  <div class="loading">
    <span></span>
  </div>
</template>

<script lang="ts" setup></script>

<style lang="scss" scoped>
.loading {
  display: inline-block;
  width: 40px;
  height: 40px;
  position: relative;
}

.loading span {
  box-sizing: border-box;
  display: block;
  position: absolute;
  width: 32px;
  height: 32px;
  margin: auto;
  border: 4px solid $color-main-dark;
  border-radius: 50%;
  border-top-color: transparent;
  animation: spin 1s linear infinite;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
}

@keyframes spin {
  to {
    transform: rotate(360deg);
  }
}
</style>
