<template>
  <section class="quran-test">
    <p class="sub-title">مسابقة السنة النبوية</p>

    <div class="flex quran-test-cards">
      <test-card
        title="المستوي الأول"
        description="متن الأحاديث من رقم (1) وحتى رقم ( 42 ) من الأربعين النووية"
        year="25 سنة"
      ></test-card>
      <test-card
        title="المستوى الثاني"
        description="متن الأحاديث من رقم (1) وحتى رقم ( 21 ) من الأربعين النووية"
        year="15 سنة"
      ></test-card>
    </div>
  </section>
</template>

<script setup>
import TestCard from "./cards/TestCard.vue";
</script>

<style scoped>
.quran-test {
  background: var(--background-1);
}
.quran-test-cards {
  flex-wrap: wrap;
  gap: 20px;
  margin-top: 2rem;
}

.sub-title {
  z-index: 1;
}
.sub-title::before {
  background: var(--color-gold-dark);
  height: 15px;
}
@media (max-width: 500px) {
}
</style>
