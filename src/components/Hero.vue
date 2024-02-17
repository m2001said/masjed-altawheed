<template>
  <div class="hero flex-col">
    <img class="hero-img" src="../assets/images/masjed-logo.svg" alt="quran icon" />
    <p class="title">مسابقات مسجد التوحيد</p>
    <p class="hero-desc">في القرآن الكريم والسنة النبوية</p>
    <a class="hero-button" href="https://forms.gle/DX18sNL8SBNZghS58" target="_blank">التسجيل في المسابقة</a>
  </div>
</template>

<script setup></script>

<style scoped>
.title {
  font-size: 2.8rem;
  font-weight: bold;
}
.hero-desc {
  font-size: 2rem;
}
.hero {
  align-items: center;
  background: url(../assets/images/pattern-background.png);
  position: relative;
  z-index: 1;
  padding: 2rem 10px;
  height: 100vh;
  gap: 10px;
}
.hero::before {
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

.hero-img {
  max-width: 150px;
  width: 100%;
}

@media (max-width: 500px) {
  .hero {
    gap: 0;
  }
  .hero-img {
    max-width: 120px;
    margin-bottom: 20px;
  }

  .title {
    font-size: 1.7rem;
  }
  .hero-desc {
    font-size: 1.3rem;
  }
}
</style>
