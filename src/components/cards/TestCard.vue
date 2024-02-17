<template>
  <div class="card flex-col">
    <div class="card-img flex">
      <img v-if="tajeweed" src="../../assets/images/quran.svg" />
      <img v-else src="../../assets/images/quran2.svg" />
    </div>
    <p class="card-title">{{ title }}</p>
    <p class="card-description">{{ description }}</p>
    <p>
      السن :
      <span> {{ year }} فما دون </span>
    </p>
    <p v-if="tajeweed">
      نسبة التجويد :
      <span> {{ tajeweed }} % </span>
    </p>
  </div>
</template>

<script setup>
defineProps(["title", "description", "tajeweed", "number", "year"]);
</script>

<style scoped>
.card {
  border: solid 1px var(--color-gold-dark);
  border-bottom-right-radius: 30px;
  border-top-left-radius: 30px;
  width: 390px;
  height: 350px;
  position: relative;
  background: var(--color-white);
  font-size: 1.3rem;
  padding: 10px;
  cursor: pointer;
  transition: all 0.3s;
}
.card:hover {
  background: var(--color-gold-light);
}
.card::before {
  content: "";
  position: absolute;
  width: 100%;
  height: 100%;
  bottom: -7px;
  right: -7px;
  background: var(--color-gold-dark);
  border-bottom-right-radius: 30px;
  border-top-left-radius: 30px;
  z-index: -1;
}

.card-img {
  background: var(--color-gold-light);
  border-radius: 50%;
  width: 90px;
  height: 90px;
}
.card-img img {
  width: 45px;
}

.card-title {
  font-size: 1.6rem;
  font-weight: bold;
  color: var(--color-gold-dark);
}
.card-description {
  font-weight: 700;
}

span {
  color: var(--color-gold-dark);
  font-weight: bold;
}

@media (max-width: 500px) {
  .card {
    width: 390px;
    font-size: 1.2rem;
    width: 100%;
    height: 100%;
    padding: 20px 10px;
  }

  .card-img {
    width: 80px;
    height: 80px;
  }
  .card-img img {
    width: 40px;
  }

  .card-title {
    font-size: 1.5rem;
  }
}
</style>
