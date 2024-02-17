<template>
  <section class="winners">
    <p class="sub-title">الفائزون</p>
    <p>سنعلن عنه بعد الانتهاء ان شاء الله</p>
  </section>
</template>

<script setup></script>

<style scoped>
.winners {
  align-items: center;
  background: url(../assets/images/pattern-background.png);
  position: relative;
  z-index: 1;
  padding: 2rem 10px;
  height: 400px;
  gap: 10px;
}
.winners::before {
  background: var(--background-1);
  content: "";
  height: 100%;
  left: 0;
  opacity: 0.7;
  position: absolute;
  top: 0;
  width: 100%;
  z-index: -11;
}
</style>
