<script setup>
</script>

<template >
  <div class="projects">
    <h1 class="heading-1 mb-30">
      <div class="circle"></div>
      <span>Latest projects</span>
    </h1>

    <ul class="projects__list list-reset">
      <li class="projects__list-item list-item">
        <div class="list-item__wrap wrap">
          <div class="wrap__top top">
            <img src="@/assets/img/figma.svg" width="48" height="48" alt="##" />
            <div class="top__name">
              <span class="descr">Alexa Dev Community Landing Page</span>
              <span class="subdescr"
                >Web UI design for alexa developers comunity</span
              >
            </div>
          </div>
          <div class="wrap__link">
            <img src="@/assets/img/figma-small.svg" width="24" alt="##" />
            <a class="link" href="https//figma.com">https//figma.com</a>
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
              alt="##"
            />
            <div class="top__name">
              <span class="descr">Portfolio Webpage</span>
              <span class="subdescr"
                >Personal Portfolio webpage with resume and blog</span
              >
            </div>
          </div>
          <div class="wrap__link">
            <img src="@/assets/img/link.svg" width="24" alt="##" />
            <a class="link" href="https://anuragyadav365.github.io"
              >https://anuragyadav365.github.io</a
            >
          </div>
        </div>
      </li>
    </ul>
  </div>
</template>


<style lang="scss" scoped>
.projects {
  margin-bottom: 45px;

  &__list {
    display: flex;
    align-items: flex-start;
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
</style>