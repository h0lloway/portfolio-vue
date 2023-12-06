<script setup>
</script>

<template >
  <div class="achievements">
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
                <img src="@/assets/img/geo.svg" width="20" alt="##" />
                Chandigarh</span
              >
            </div>
            <div class="left__place">
              <img src="@/assets/img/alexa.svg" width="43" alt="##" />
              <div class="left__name">
                <span class="descr">Graphic Designer</span>
                <span class="subdescr">Alexa Dev Community</span>
              </div>
            </div>
          </div>
          <div class="wrap__text">
            Creatively Designing and Developing web UI for Chandigarh
            University’s Alexa Developer Community, upcoming big launch of full
            website.
          </div>
        </div>
      </li>
      <li class="achievements__list-item list-item">
        <div class="list-item__wrap wrap">
          <div class="wrap__left left">
            <div class="left__date">
              <div class="small-circle"></div>
              <span>Oct 2021 - Nov 2021</span>
              <span class="locate">
                <img src="@/assets/img/geo.svg" width="20" alt="##" />
                Online</span
              >
            </div>
            <div class="left__place">
              <img src="@/assets/img/github1.svg" width="43" alt="##" />
              <div class="left__name">
                <span class="descr">Hacktoberfest Contributor</span>
                <span class="subdescr">Github</span>
              </div>
            </div>
          </div>
          <div class="wrap__text">
            Contributed 8 PR’s in various open source projects. Great experience
            and learning alot about working with Github and open-source.
            Connecting with developers
          </div>
        </div>
      </li>
      <li class="achievements__list-item list-item">
        <div class="list-item__wrap wrap">
          <div class="wrap__left left">
            <div class="left__date">
              <div class="small-circle"></div>
              <span>Jan 2021 - March 2021</span>
              <span class="locate">
                <img src="@/assets/img/geo.svg" width="20" alt="##" />
                Online</span
              >
            </div>
            <div class="left__place">
              <img src="@/assets/img/winter.svg" width="43" alt="##" />
              <div class="left__name">
                <span class="descr">Contributor</span>
                <span class="subdescr">Winter of Code</span>
              </div>
            </div>
          </div>
          <div class="wrap__text">
            Overwhelming to be a part of DSC NSEC project - DSC NSEC Algorithms
            for Winter of Code 2020. First introduction to Git and Github. How
            github is used by most of the programmers in order to manage the
            projects.
          </div>
        </div>
      </li>
      <li class="achievements__list-item list-item">
        <div class="list-item__wrap wrap">
          <div class="wrap__left left">
            <div class="left__date">
              <div class="small-circle"></div>
              <span>Oct 2020 - Dec 2020</span>
              <span class="locate">
                <img src="@/assets/img/geo.svg" width="20" alt="##" />
                Online</span
              >
            </div>
            <div class="left__place">
              <img src="@/assets/img/google.svg" width="43" alt="##" />
              <div class="left__name">
                <span class="descr">30Days of Google Cloud</span>
                <span class="subdescr">Google</span>
              </div>
            </div>
          </div>
          <div class="wrap__text">
            Hands on practice on Google Cloud Platform - the tool that powers
            apps like Google Search, Gmail and YouTube. As part of the program
            had learned the concepts like computing, application development,
            big data & machine learning using cloud.
          </div>
        </div>
      </li>
    </ul>
  </div>
</template>


<style lang="scss" scoped>
.achievements {
  margin-bottom: 45px;

  &__list {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    width: 100%;

    border-left: 1px solid #ddeafc;
  }

  .list-item {
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
          font: 400 12px/128% "DM Sans", sans-serif;
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
          font: 400 14px/128% "DM Sans", sans-serif;
          letter-spacing: 0.136px;
        }
        .subdescr {
          color: #2e2e48;
          font: 500 16px/128% "DM Sans", sans-serif;
        }
      }

      &__text {
        width: 60%;
        color: #47516b;
        font: 400 14px/128% "DM Sans", sans-serif;
        letter-spacing: 0.117px;
      }
    }
  }
  .list-item:not(:last-child) {
    margin-bottom: 10px;
  }
}
</style>