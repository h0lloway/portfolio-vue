<script setup>
import { ref } from "vue";

// const items = ref([
//   {
//     mainimg: "skillbox-logo",
//     name: "Образовательная платформа Skillbox",
//     descr: "Профессия Frontend-разработчик",
//   },
//   {
//     mainimg: "dstu",
//     name: "Донской Государственный Технический Университет",
//     descr: "Кафедра «Технология Машиностроения",
//   },
// ]);

const props = defineProps({
  mainimg: {
    type: String,
    required: true,
  },
  name: {
    type: Boolean,
    default: "Name",
  },
  descr: {
    type: Boolean,
    default: "Descr",
  },
});
</script>

<template>
  <li class="skills__list-item list-item">
    <!-- v-for="item in items" :key="item.name" -->
    <div class="list-item__wrap">
      <img
        :class="['wrap-img']"
        :src="'/assets/img/' + mainimg + '.svg'"
        :alt="mainimg"
      />
      <div :class="['tools-name']">{{ name }}</div>
      <div :class="['tools-descr']">{{ descr }}</div>
    </div>
  </li>
</template>

<style lang="scss" scoped>
.list-item {
  display: block;
  background: #ebf2fc;
  // flex: 0 0 20%;

  &__wrap {
    padding: 20px;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: center;
    text-align: center;
    height: 100%;

    .wrap-img {
      width: 60px;
    }

    .tools-name {
      margin-top: 15px;
      margin-bottom: 10px;
      color: #2e2e48;
      font: 500 16px/128% "Manrope", sans-serif;
    }
    .tools-descr {
      color: var(--gray-default, #79819a);
      font: 400 12px/128% "Manrope", sans-serif;
      letter-spacing: 0.101px;
    }
  }
}

@media screen and (max-width: 1300px) {
  .skills {
    .list-item {
      border-radius: 0;
    }
  }
}

@media screen and (max-width: 1100px) {
  .skills {
    .list-item {
      border-radius: 0;
    }
  }
}

@media screen and (max-width: 500px) {
  .skills {
    .list-item {
      &__wrap {
        padding: 20px 10px;

        img {
          width: 40px;
        }

        .tools-descr {
          width: 80%;
        }
      }
    }
  }
}
</style>