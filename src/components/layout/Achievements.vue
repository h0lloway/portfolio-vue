<script setup>
import ContentTitle from "@/components/ContentTitle.vue";
import Divider from "@/components/Divider.vue";
import AchievementsCard from "@/components/AchievementsCard.vue";
</script>

<template >
  <div class="achievements">
    <Divider :class="['achievements__divider']" />

    <div class="achievements__content content-common">
      <ContentTitle title="Achievements" />

      <ul class="achievements__list list-reset">
        <AchievementsCard :class="['bg-color']"
          live="Present"
          locatetext="Online"
          descr="Frontend-developer"
          subdescr="МТС Финтех"
          text="Lorem ipsum dolor sit amet consectetur adipisicing elit. Quo sequi
              facilis nostrum, culpa, dignissimos dicta aliquid ut commodi
              aspernatur harum voluptatum enim libero."
          locateimg="geo"
          mainimg="MTC"
        />

        <AchievementsCard
          live="Dec 2022 - Jule 2023"
          locatetext="Online"
          descr="Frontend-developer"
          subdescr="Актион"
          text="Lorem ipsum dolor sit amet consectetur adipisicing elit. Quo sequi
              facilis nostrum, culpa, dignissimos dicta aliquid ut commodi
              aspernatur harum voluptatum enim libero."
          locateimg="geo"
          mainimg="action"
        />

        <AchievementsCard
          live="April 2022 - Dec 2022"
          locatetext="Online"
          descr="HTML coder"
          subdescr="Adcome labs"
          text="Lorem ipsum dolor sit amet consectetur adipisicing elit. Quo sequi
              facilis nostrum, culpa, dignissimos dicta aliquid ut commodi
              aspernatur harum voluptatum enim libero."
          locateimg="geo"
          mainimg="adcome"
        />
      </ul>
    </div>
  </div>
</template>


<style lang="scss" scoped>
.achievements {
  display: flex;

  &__content {
    margin-bottom: 40px;
  }

  &__list {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    width: 100%;
  }
}
</style>