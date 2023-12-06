<script setup>
</script>

<template >
  <div class="education">
    <h1 class="heading-1 mb-30">
      <div class="circle"></div>
      <span>Education</span>
    </h1>

    <ul class="education__list list-reset">
      <li class="education__list-item list-item">
        <div class="list-item__wrap wrap">
          <div class="wrap__name">
            <img src="@/assets/img/univ1.svg" width="40" alt="##" />
            <span>Chandigarh University</span>
          </div>
          <div class="wrap__descr">
            Bachelor in Computer Science Engineering
          </div>
          <div class="wrap__date">2020 - 2024</div>
          <div class="wrap__percent"><span>Percentage</span> - 9 CGPA</div>
        </div>
      </li>
      <li class="education__list-item list-item">
        <div class="list-item__wrap wrap">
          <div class="wrap__name">
            <img src="@/assets/img/univ2.svg" width="47" alt="##" />
            <span>Suditi Global Academy</span>
          </div>
          <div class="wrap__descr">Intermediate XI - XII(CBSE)</div>
          <div class="wrap__date">2018-2020</div>
          <div class="wrap__percent"><span>Percentage</span> - 85%</div>
        </div>
      </li>
      <li class="education__list-item list-item">
        <div class="list-item__wrap wrap">
          <div class="wrap__name">
            <img src="@/assets/img/univ3.svg" width="46" alt="##" />
            <span>Akanksha Global Acadmey</span>
          </div>
          <div class="wrap__descr">High School IX - X(CBSE)</div>
          <div class="wrap__date">2016-2018</div>
          <div class="wrap__percent"><span>Percentage</span> - 92%</div>
        </div>
      </li>
    </ul>
  </div>
</template>


<style lang="scss" scoped>
.education {
  margin-bottom: 45px;

  &__list {
    display: flex;
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
        font: 400 12px/128% "DM Sans", sans-serif;
        letter-spacing: 0.101px;
      }

      &__percent {
        font: 400 14px/128% "DM Sans", sans-serif;
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
</style>