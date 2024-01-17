<script setup>
import ContentTitle from "@/components/ContentTitle.vue";
import Divider from "@/components/Divider.vue";
import EducationCard from "@/components/EducationCard.vue";
</script>

<template >
  <div class="education">
    <Divider :class="['education__divider']" />

    <div class="education__content content-common">
      <ContentTitle :class="['education__title']" title="Education" />

      <ul class="education__list list-reset">
        <EducationCard
          :class="['color-logo']"
          name="Образовательная платформа Skillbox"
          images="skillbox-logo"
          descr="Профессия Frontend&#8209;разработчик"
          date="2021-2022"
        />

        <EducationCard
          name="Донской Государственный Технический Университет"
          images="dstu"
          descr="Кафедра «Технология Машиностроения»"
          date="2013-2015"
        />
      </ul>
    </div>
  </div>
</template>


<style lang="scss" scoped>
.education {
  display: flex;

  &__list {
    display: flex;
    flex-wrap: wrap;
    margin-left: -5px;
    margin-right: -5px;
    margin-bottom: 30px;
  }
}

@media screen and (max-width: 1300px) {
  .education {
    &__list {
      flex-direction: column;
    }
  }
}
</style>