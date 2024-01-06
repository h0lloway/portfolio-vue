<script setup>
</script>

<template >
  <div class="education">
    <div class="education__divider divider">
      <div class="divider__circle">
        <div class="divider__circle-inside">
          <div class="divider__circle-inside-viol"></div>
        </div>
      </div>
      <div class="divider__line"></div>
    </div>

    <div class="education__content content-common">
      <h1 class="heading-1 mb-30">
        <div class="circle"></div>
        <span>Education</span>
      </h1>

      <ul class="education__list list-reset">
        <li class="education__list-item list-item">
          <div class="list-item__wrap wrap">
            <div class="wrap__name">
              <img
                style="
                  border: 0.4px solid #cacaca;
                  height: 47px;
                  padding: 0 5px;
                  border-radius: 15px;
                "
                src="@/assets/img/skillbox-logo.svg"
                width="47"
                alt="logo"
              />
              <span
                >Образовательная <br />
                платформа Skillbox</span
              >
            </div>
            <div class="wrap__descr">Профессия Frontend&#8209;разработчик</div>
            <div class="wrap__date">2021-2022</div>
          </div>
        </li>
        <li class="education__list-item list-item">
          <div class="list-item__wrap wrap">
            <div class="wrap__name">
              <img src="@/assets/img/DSTU1.png" width="46" alt="logo" />
              <span>Донской Государственный Технический Университет</span>
            </div>
            <div class="wrap__descr">Кафедра «Технология Машиностроения»</div>
            <div class="wrap__date">2013-2015</div>
          </div>
        </li>
      </ul>
    </div>
  </div>
</template>


<style lang="scss" scoped>
.education {
  display: flex;

  &__list {
    display: flex;
    margin-bottom: 30px;
  }
  .list-item {
    flex: 1 1 33%;
    background: #ebf2fc;

    .wrap {
      height: 100%;
      display: flex;
      flex-direction: column;
      justify-content: space-between;
      padding: 20px;

      &__name {
        display: flex;
        align-items: center;
        margin-bottom: 10px;

        span {
          padding-left: 15px;
        }
      }

      &__descr {
        margin-bottom: 10px;
      }

      &__date {
        margin-bottom: 10px;
        color: #79819a;
        font: 400 12px/128% "Manrope", sans-serif;
        letter-spacing: 0.101px;
      }

      &__percent {
        font: 400 14px/128% "Manrope", sans-serif;
        letter-spacing: 0.121px;

        span {
          color: #5d5fef;
        }
      }
    }
  }
  .list-item:first-child {
    border-radius: 10px 0 0 10px;
  }
  .list-item:last-child {
    border-radius: 0 10px 10px 0;
  }
  .list-item:not(:last-child) {
    margin-right: 10px;
  }
}

@media screen and (max-width: 1300px) {
  .education {
    &__list {
      flex-direction: column;
    }

    .list-item:not(:last-child) {
      margin: 0;
      margin-bottom: 10px;
    }

    .list-item:first-child {
      border-radius: 10px 10px 0 0;
    }

    .list-item:last-child {
      border-radius: 0 0 10px 10px;
    }
  }
}

@media screen and (max-width: 1300px) {
  .education {
    .list-item {
      .wrap {
        padding: 15px;
      }
    }
  }
}
</style>