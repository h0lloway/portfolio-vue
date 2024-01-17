<script setup>
const props = defineProps({
  descr: {
    type: Boolean,
    default: "Descr",
  },
  subdescr: {
    type: Boolean,
    default: "Subdescr",
  },
  logoimg: {
    type: String,
    required: true,
  },
  linktext: {
    type: String,
    required: true,
  },
	link: {
    type: String,
    required: true,
  },
  linkimg: {
    type: String,
    required: true,
  },
});
</script>

<template>
  <li class="projects__list-item list-item">
    <div class="list-item__wrap wrap">
      <div class="wrap__top top">
        <img
          :class="['top__img']"
          :src="'/assets/img/' + logoimg + '.svg'"
          :width="48"
          :alt="logoimg"
        />
        <div class="top__name">
          <span class="descr"> {{ descr }} </span>
          <span class="subdescr"> {{ subdescr }} </span>
        </div>
      </div>
      <div class="wrap__link">
        <img
          :src="'/assets/img/' + linkimg + '.svg'"
          :width="24"
          :alt="linkimg"
        />
        <a :href="link" :class="['link']" :target="['_blank']">
          {{ linktext }}
        </a>
      </div>
    </div>
  </li>
</template>

<style lang="scss" scoped>
.list-item {
  flex: 0 0 50%;
  padding: 5px 5px;

  .wrap {
    height: 100%;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    background: #ebf2fc;
    padding: 20px;

    &__link {
      margin-top: 15px;
      display: flex;
      align-items: center;

      a {
        padding-left: 5px;
      }
    }
    .top {
      display: flex;
      align-items: center;

      &__name {
        padding-left: 15px;
      }
    }
  }
}
.list-item:first-child .wrap {
  border-radius: 10px 0 0 10px;
}
.list-item:last-child .wrap {
  border-radius: 0 10px 10px 0;
}

@media screen and (max-width: 1600px) {
  .list-item:first-child .wrap {
    border-radius: 10px 10px 0 0;
  }

  .list-item:last-child .wrap {
    border-radius: 0 0 10px 10px;
  }
}

@media screen and (max-width: 500px) {
  .wrap {
    .top {
      min-height: 48px;
      &__name {
        padding-left: 9px;
      }
    }
  }
}
</style>