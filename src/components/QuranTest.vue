<template>
  <section class="quran-test">
    <p class="sub-title">مسابقة القرآن الكريم</p>

    <div class="flex quran-test-cards">
      <test-card title="مستوي الحفاظ" description="القرآن الكريم كاملا" tajeweed="25" year="30 سنة"></test-card>
      <test-card title="المستوي الأول" description="القرآن الكريم كاملا" tajeweed="10" year="25 سنة"></test-card>
      <test-card
        title="المستوى الثاني"
        description="عشرين جزءاً ( من سورة الناس إلى سورة يونس )"
        tajeweed="10"
        year="18 سنة"
      ></test-card>
      <test-card
        title="المستوى الثالث"
        description="خمسة عشر جزءاً ( من سورة الناس إلى سورة الـكهف )"
        tajeweed="10"
        year="15 سنة"
      ></test-card>
      <test-card
        title="المستوى الرابع"
        description="عشرة أجزاء ( من سورة الناس إلى سورة العنكبوت )"
        tajeweed="10"
        year="13 سنة"
      ></test-card>
      <test-card
        title="المستوى الخامس"
        description="خمسة أجزاء ( من سورة الناس إلى سورة الأحقاف )"
        tajeweed="5"
        year="11 سنة"
      ></test-card>
      <test-card
        title="المستوى السادس"
        description="ثلاثة أجزاء ( من سورة الناس إلى سورة المجادلة )"
        tajeweed="5"
        year="9 سنوات"
      ></test-card>
    </div>
  </section>
</template>

<script setup>
import TestCard from "./cards/TestCard.vue";
</script>

<style scoped>
.quran-test {
  margin-bottom: 2rem;
}
.quran-test-cards {
  flex-wrap: wrap;
  gap: 40px;
  margin-top: 2rem;
}
</style>
