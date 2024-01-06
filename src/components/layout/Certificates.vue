<script setup>
</script>

<template >
  <div class="certificates">
    <div class="certificates__divider divider">
      <div class="divider__circle">
        <div class="divider__circle-inside">
          <div class="divider__circle-inside-viol"></div>
        </div>
      </div>
      <div class="divider__line"></div>
    </div>

    <div class="certificates__content content-common">
      <h1 class="heading-1 mb-30">
        <div class="circle"></div>
        <span>Certificates & Awards</span>
      </h1>

      <ul class="certificates__list list-reset">
        <li class="certificates__list-item list-item">
          <div class="list-item__wrap wrap">
            <div class="wrap__left left">
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
              <div class="left__name">
                <span class="descr">Skillbox</span>
                <span class="subdescr">Frontend-developer</span>
              </div>
            </div>
            <div class="wrap__date">Dec&#160;2021 - Aug&#160;2022</div>
          </div>
        </li>
      </ul>
    </div>
  </div>
</template>


<style lang="scss" scoped>
.certificates {
  display: flex;

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
    border-radius: 10px;

    .wrap {
      display: flex;
      justify-content: space-between;
      align-items: center;

      .left {
        display: flex;
        align-items: center;

        &__name {
          padding-left: 15px;
        }

        .descr {
          color: #79819a;
          font: 400 14px/128% 'Manrope', sans-serif;
          letter-spacing: 0.136px;
        }
        .subdescr {
          color: #2e2e48;
          font: 500 16px/128% 'Manrope', sans-serif;
        }
      }

      &__date {
        padding-left: 15px;
        color: #47516b;
        font: 400 14px/128% 'Manrope', sans-serif;
        letter-spacing: 0.117px;
      }
    }
  }
  .list-item:not(:last-child) {
    margin-bottom: 10px;
  }
}

@media screen and (max-width: 1300px) {
  .certificates {

    .list-item {
      padding: 20px 20px;
    }
  }
}


</style>