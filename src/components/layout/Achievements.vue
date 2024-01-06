<script setup>
</script>

<template >
  <div class="achievements">
    <div class="achievements__divider divider">
      <div class="divider__circle">
        <div class="divider__circle-inside">
          <div class="divider__circle-inside-viol"></div>
        </div>
      </div>
      <div class="divider__line"></div>
    </div>

    <div class="achievements__content content-common">
      <h1 class="heading-1 mb-30">
        <div class="circle"></div>
        <span>Achievements</span>
      </h1>

      <ul class="achievements__list list-reset">
        <li class="achievements__list-item list-item">
          <div class="list-item__wrap wrap">
            <div class="wrap__left left">
              <div class="left__date">
                <div class="small-circle"></div>
                <span class="live">Present</span>
                <span class="locate">
                  <img
                    src="@/assets/img/geo.svg"
                    width="20"
                    alt="online"
                  />Online</span
                >
              </div>
              <div class="left__place">
                <img src="@/assets/img/MTC.svg" width="43" alt="logo" />
                <div class="left__name">
                  <span class="descr">Frontend-developer</span>
                  <span class="subdescr">МТС Финтех</span>
                </div>
              </div>
            </div>
            <div class="wrap__text">
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Quo sequi
              facilis nostrum, culpa, dignissimos dicta aliquid ut commodi
              aspernatur harum voluptatum enim libero.
            </div>
          </div>
        </li>

        
        <li class="achievements__list-item list-item">
          <div class="list-item__wrap wrap">
            <div class="wrap__left left">
              <div class="left__date">
                <div class="small-circle"></div>
                <span>Dec 2022 - Jule 2023</span>
                <span class="locate">
                  <img src="@/assets/img/geo.svg" width="20" alt="online" />
                  Online</span
                >
              </div>
              <div class="left__place">
                <img
                  src="@/assets/img/action.jpeg"
                  width="43"
                  alt="logo"
                  style="border-radius: 100%"
                />
                <div class="left__name">
                  <span class="descr">Frontend-developer</span>
                  <span class="subdescr">Актион</span>
                </div>
              </div>
            </div>
            <div class="wrap__text">
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Quo sequi
              facilis nostrum, culpa, dignissimos dicta aliquid ut commodi
              aspernatur harum voluptatum enim libero.
            </div>
          </div>
        </li>
        <li class="achievements__list-item list-item">
          <div class="list-item__wrap wrap">
            <div class="wrap__left left">
              <div class="left__date">
                <div class="small-circle"></div>
                <span>April 2022 - Dec 2022</span>
                <span class="locate">
                  <img src="@/assets/img/geo.svg" width="20" alt="online" />
                  Online</span
                >
              </div>
              <div class="left__place">
                <img
                  src="@/assets/img/adcome.jpeg"
                  width="43"
                  alt="logo"
                  style="border-radius: 100%"
                />
                <div class="left__name">
                  <span class="descr">HTML coder</span>
                  <span class="subdescr">Adcome labs</span>
                </div>
              </div>
            </div>
            <div class="wrap__text">
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Quo sequi
              facilis nostrum, culpa, dignissimos dicta aliquid ut commodi
              aspernatur harum voluptatum enim libero.
            </div>
          </div>
        </li>
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

  .list-item {
    position: relative;
    padding: 20px 35px;
    width: 100%;

    .wrap {
      display: flex;
      justify-content: space-between;
      align-items: center;

      .left {
        display: flex;
        flex-direction: column;

        &__date {
          display: flex;
          align-items: center;
          position: relative;
          margin-bottom: 8px;
          color: #47516b;
          font: 400 12px/128% "Manrope", sans-serif;
          letter-spacing: 0.101px;

          .live {
            color: #9251f7;
            background: #efe2f9;
            padding: 3px;
            border-radius: 4px;
          }

          .locate {
            display: inline-flex;
            align-items: center;
            padding-left: 7px;
          }
        }

        &__place {
          display: flex;
        }

        &__name {
          padding-left: 15px;
        }

        .descr {
          color: #79819a;
          font: 400 14px/128% "Manrope", sans-serif;
          letter-spacing: 0.136px;
        }
        .subdescr {
          color: #2e2e48;
          font: 500 16px/128% "Manrope", sans-serif;
        }
      }

      &__text {
        width: 60%;
        color: #47516b;
        font: 400 14px/128% "Manrope", sans-serif;
        letter-spacing: 0.117px;
      }
    }
  }

  .list-item::before {
    position: absolute;
    content: "";
    width: 1px;
    height: 85%;
    background: #ededed;
    top: 39px;
    left: -1px;
  }
  .list-item:not(:last-child) {
    margin-bottom: 10px;
  }

  .list-item:last-child::before {
    height: 60%;
  }
}

@media screen and (max-width: 1300px) {
  .achievements {
    .list-item {
      .wrap {
        display: block;

        &__text {
          margin-top: 15px;
          width: 100%;
        }
      }
    }
  }
}
</style>