<script setup>
</script>

<template >
  <div class="skills">
    <h1 class="heading-1 mb-30">
      <div class="circle"></div>
      <span>Tools/Skills</span>
    </h1>

    <ul class="skills__list list-reset">
      <li class="skills__list-item item1 list-item">
        <div class="list-item__wrap">
          <img src="@/assets/img/html.svg" width="40" alt="##" />
          <div class="tools-name">HTML5</div>
          <div class="tools-descr">Structural Design</div>
        </div>
      </li>
      <li class="skills__list-item item2 list-item">
        <div class="list-item__wrap">
          <img src="@/assets/img/css.svg" width="55" alt="##" />
          <div class="tools-name">CSS3</div>
          <div class="tools-descr">Style Design</div>
        </div>
      </li>
      <li class="skills__list-item item3 list-item">
        <div class="list-item__wrap">
          <img src="@/assets/img/wordpress.svg" width="67" alt="##" />
          <div class="tools-name">Wordpress</div>
          <div class="tools-descr">Web development</div>
        </div>
      </li>
      <li class="skills__list-item item4 list-item">
        <div class="list-item__wrap">
          <img src="@/assets/img/vscode.svg" width="40" alt="##" />
          <div class="tools-name">VS Code</div>
          <div class="tools-descr">Code editor</div>
        </div>
      </li>
      <li class="skills__list-item item5 list-item">
        <div class="list-item__wrap">
          <img src="@/assets/img/notion.svg" width="40" alt="##" />
          <div class="tools-name">Notion</div>
          <div class="tools-descr">Project managment</div>
        </div>
      </li>
      <li class="skills__list-item item6 list-item">
        <div class="list-item__wrap">
          <img src="@/assets/img/figma.svg" width="48" alt="##" />
          <div class="tools-name">Figma</div>
          <div class="tools-descr">Web UI Design, Prototyping</div>
        </div>
      </li>
      <li class="skills__list-item item7 list-item">
        <div class="list-item__wrap">
          <img src="@/assets/img/java.svg" width="70" alt="##" />
          <div class="tools-name">Java</div>
          <div class="tools-descr">Software Development</div>
        </div>
      </li>
      <li class="skills__list-item item8 list-item">
        <div class="list-item__wrap">
          <img src="@/assets/img/python.svg" width="60" alt="##" />
          <div class="tools-name">Python</div>
          <div class="tools-descr">Design workspace</div>
        </div>
      </li>
    </ul>
  </div>
</template>


<style lang="scss" scoped>
.skills {
  margin-bottom: 45px;

  &__list {

    display: grid;
    grid-template-columns: repeat(15, 1fr);
    grid-template-rows: repeat(6, 1fr);
    grid-column-gap: 10px;
    grid-row-gap: 10px;

    .item1 {
      grid-area: 4 / 1 / 7 / 4;
      border-radius: 0px 0px 0px 10px;
    }
    .item2 {
      grid-area: 4 / 4 / 7 / 7;
    }
    .item3 {
      grid-area: 4 / 7 / 7 / 10;
    }
    .item4 {
      grid-area: 4 / 10 / 7 / 13;
    }
    .item5 {
      grid-area: 4 / 13 / 7 / 16;
      border-radius: 0px 0px 10px 0px;
    }
    .item6 {
      grid-area: 1 / 1 / 4 / 6;
      border-radius: 10px 0px 0px 0px;
    }
    .item7 {
      grid-area: 1 / 6 / 4 / 11;
    }
    .item8 {
      grid-area: 1 / 11 / 4 / 16;
      border-radius: 0px 10px 0px 0px;
    }
  }

  .list-item {
    display: block;
    background: #ebf2fc;

    &__wrap {
      padding: 20px;
      display: flex;
      flex-direction: column;
      justify-content: space-between;
      align-items: center;
      text-align: center;
      height: 100%;

      .tools-name {
        margin-top: 15px;
        margin-bottom: 10px;
        color: #2e2e48;
        font-family: DM Sans;
        font: 500 16px/128% "DM Sans", sans-serif;
      }
      .tools-descr {
        color: var(--gray-default, #79819a);
        font-family: DM Sans;
        font: 400 12px/128% "DM Sans", sans-serif;
        letter-spacing: 0.101px;
      }
    }
  }
}
</style>