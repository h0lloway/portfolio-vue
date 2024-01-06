<script setup>
</script>

<template >
  <div class="projects">
    <div class="projects__divider divider">
      <div class="divider__circle">
        <div class="divider__circle-inside">
          <div class="divider__circle-inside-viol"></div>
        </div>
      </div>
      <div class="divider__line"></div>
    </div>

    <div class="projects__content content-common">
      <h1 class="heading-1 mb-30">
        <div class="circle"></div>
        <span>Latest projects</span>
      </h1>

      <ul class="projects__list list-reset">
        <li class="projects__list-item list-item">
          <div class="list-item__wrap wrap">
            <div class="wrap__top top">
              <img
                src="@/assets/img/webpage.svg"
                width="48"
                height="48"
                alt="logo"
              />
              <div class="top__name">
                <span class="descr">Portfolio Webpage</span>
                <span class="subdescr">
                  Personal Portfolio webpage with resume</span
                >
              </div>
            </div>
            <div class="wrap__link">
              <img src="@/assets/img/link.svg" width="24" alt="link" />
              <a
                class="link"
                href="https://coruscating-clafoutis-22da2b.netlify.app/"
                target="_blank"
                >LINK to project</a
              >
            </div>
          </div>
        </li>
        <li class="projects__list-item list-item">
          <div class="list-item__wrap wrap">
            <div class="wrap__top top">
              <img
                src="@/assets/img/webpage.svg"
                width="48"
                height="48"
                alt="logo"
              />
              <div class="top__name">
                <span class="descr">SitDownPls Webpage</span>
                <span class="subdescr"
                  >Сайт магазина мебели (учебный проект)</span
                >
              </div>
            </div>
            <div class="wrap__link">
              <img src="@/assets/img/link.svg" width="24" alt="link" />
              <a
                class="link"
                href="https://h0lloway.github.io/SitDownPls__makdu/"
                target="_blank"
                >LINK to project</a
              >
            </div>
          </div>
        </li>
      </ul>
    </div>
  </div>
</template>


<style lang="scss" scoped>
.projects {
  display: flex;

  &__list {
    display: flex;
    align-items: flex-start;

    margin-bottom: 30px;
  }
  .list-item {
    flex: 1 1 50%;
    padding: 20px;
    background: #ebf2fc;

    .wrap {
      height: 100%;
      display: flex;
      flex-direction: column;

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
        min-height: 68px;

        &__name {
          padding-left: 15px;
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
  .projects {
    &__list {
      flex-direction: column;
    }

    &__list-item {
      width: 100%;
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

@media screen and (max-width: 500px) {
  .projects {
    .list-item {
      padding: 15px;
      .wrap {
        .top {
          min-height: 48px;
          &__name {
            padding-left: 9px;
          }
        }
      }
    }
  }
}
</style>