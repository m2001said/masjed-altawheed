<template>
  <navbar></navbar>
  <hero></hero>
  <quran-test></quran-test>
  <hadith-test></hadith-test>
  <instructions></instructions>
  <test-date></test-date>
  <winners></winners>
  <Footer></Footer>
</template>

<script setup>
import Navbar from "./components/Navbar.vue";
import Hero from "./components/Hero.vue";
import QuranTest from "./components/QuranTest.vue";
import HadithTest from "./components/HadithTest.vue";
import Instructions from "./components/Instructions.vue";
import TestDate from "./components/TestDate.vue";
import Winners from "./components/Winners.vue";
import Footer from "./components/Footer.vue";

setTimeout(() => {
  // intersection observer
  const animatedElements = document.querySelectorAll(".add-animation");
  const options = {};
  const observer = new IntersectionObserver((entries) => {
    entries.forEach((entry) => {
      const animationClass = entry.target.getAttribute("animation-class");
      const animationClassArr = animationClass.split(" ");

      if (entry.isIntersecting) {
        animationClassArr.forEach((c) => {
          entry.target.classList.add(c);
        });
      } else {
        animationClassArr.forEach((c) => {
          entry.target.classList.remove(c);
        });
      }
    });
  }, options);
  animatedElements.forEach((element) => {
    observer.observe(element);
  });
}, 2000);
</script>

<style scoped></style>
