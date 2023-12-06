<script setup>
</script>

<template >
  <div class="certificates">
    <h1 class="heading-1 mb-30">
      <div class="circle"></div>
      <span>Certificates & Awards</span>
    </h1>

    <ul class="certificates__list list-reset">
      <li class="certificates__list-item list-item">
        <div class="list-item__wrap wrap">
          <div class="wrap__left left">
            <img src="@/assets/img/award1.svg" width="43" alt="##" />
            <div class="left__name">
              <span class="descr">freeCodeCamp</span>
              <span class="subdescr">Responsive Web Design</span>
            </div>
          </div>
          <div class="wrap__date">Dec 2021 - Feb 2022</div>
        </div>
      </li>
      <li class="certificates__list-item list-item">
        <div class="list-item__wrap wrap">
          <div class="wrap__left left">
            <img src="@/assets/img/google.svg" width="43" alt="##" />
            <div class="left__name">
              <span class="descr">Data Strcture & Algorithms</span>
              <span class="subdescr">Google</span>
            </div>
          </div>
          <div class="wrap__date">Mar 2021 - Jun 2021</div>
        </div>
      </li>
    </ul>
  </div>
</template>


<style lang="scss" scoped>
.certificates {
  margin-bottom: 45px;

  &__list {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    width: 100%;
  }

  .list-item {
    padding: 20px 35px;
    width: 100%;
    background: #ebf2fc;

    .wrap {
      display: flex;
      justify-content: space-between;
      align-items: center;

      .left {
        display: flex;

        &__name {
          padding-left: 15px;
        }

        .descr {
          color: #79819a;
          font: 400 14px/128% "DM Sans", sans-serif;
          letter-spacing: 0.136px;
        }
        .subdescr {
          color: #2e2e48;
          font: 500 16px/128% "DM Sans", sans-serif;
        }
      }

      &__date {
        color: #47516b;
        font: 400 14px/128% "DM Sans", sans-serif;
        letter-spacing: 0.117px;
      }
    }
  }

  .list-item:first-child {
    border-radius: 10px 10px 0 0;
  }
  .list-item:last-child {
    border-radius: 0 0 10px 10px;
  }
  .list-item:not(:last-child) {
    margin-bottom: 10px;
  }
}
</style>