<template>
  <section class="instruction flex-col">
    <p class="sub-title">تنبيهات المسابقة</p>

    <ol class="list">
      <li>
        يسمح بالمشاركة في أول خمس مستويات من مسابقة القرآن الكريم ومستويات مسابقة السنة النبوية لأبناء إحدى القرى
        التالية : ( المسلمي ، صبيح ، الزرزمون ، الفواقسة ، كفر عجيبة ، عزبة موسى ، عزبة البيه ، عزبة رأفت ، أبو شحاته ،
        المساعدة ، الشيخ منصور ، جهينة ، مختار بك )
      </li>
      <li>يسمح بالمشاركة في المستويين الخامس والسادس من مسابقة القرآن الكريم لأبناء قرية المسلمي فقط</li>
      <li>لا يسمح للفائزين في السنوات السابقة في أي مستوى ، المشاركة في نفس المستوى أو أي مستوى أقل منه</li>
      <li>يمكن للمشاركين التسجيل في مسابقتي القرآن الكريم والسنة النبوية معا .</li>
      <li>نسبة النجاح في مسابقة القرآن الكريم هي ٨٥ ٪</li>
      <li>
        التسجيل لا يعني القبول في المسابقة حيث ستتم مراجعة بيانات المشاركين ومطابقتها للشروط ثم إعلان أسماء المشاركين
      </li>
    </ol>
  </section>
</template>

<script setup></script>

<style scoped>
.instruction {
  background: var(--color-gold-dark);
}
.sub-title {
  margin-bottom: 20px;
  z-index: 1;
}
ol {
  margin: 0;
  padding: 0 50px;
}
.list li {
  font-size: 1.2rem;
  font-weight: 700;
  margin-bottom: 10px;
  line-height: 1.4;
  text-align: right;
}
@media (max-width: 500px) {
  ol {
    padding: 0 20px 0 0;
  }
}
</style>
