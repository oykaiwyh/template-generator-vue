<template>
  <a-layout class="container">
    <a-layout-header>
      <Header></Header>
    </a-layout-header>
    <a-layout-content>
      <slot></slot>
    </a-layout-content>
    <a-layout-footer class="footer-wrapper">
      <Footer></Footer>
    </a-layout-footer>
  </a-layout>
</template>

<script setup lang="ts">
</script>

<style>
@import './index.scss';
</style>