<script setup>
</script>

<template >
  <div class="skills">
    <div class="skills__divider divider">
      <div class="divider__circle">
        <div class="divider__circle-inside">
          <div class="divider__circle-inside-viol"></div>
        </div>
      </div>
      <div class="divider__line"></div>
    </div>

    <div class="skills__content content-common">
      <h1 class="heading-1 mb-30">
        <div class="circle"></div>
        <span>Tools/Skills</span>
      </h1>

      <ul class="skills__list list-reset">
        <li class="skills__list-item item1 list-item">
          <div class="list-item__wrap">
            <img src="@/assets/img/figma.svg" alt="figma" />
            <div class="tools-name">Figma</div>
            <div class="tools-descr">Верстка по макетам Figma</div>
          </div>
        </li>
        <li class="skills__list-item item2 list-item">
          <div class="list-item__wrap">
            <img src="@/assets/img/gulp.svg" alt="gulp" />
            <div class="tools-name">Gulp</div>
            <div class="tools-descr">Быстрый сборщик проектов</div>
          </div>
        </li>
        <li class="skills__list-item item3 list-item">
          <div class="list-item__wrap">
            <img src="@/assets/img/git.svg" alt="git" />
            <div class="tools-name">Git</div>
            <div class="tools-descr">
              Система контроля <br />
              версий
            </div>
          </div>
        </li>
        <li class="skills__list-item item4 list-item">
          <div class="list-item__wrap">
            <img src="@/assets/img/vscode.svg" alt="vsc" />
            <div class="tools-name">VS Code</div>
            <div class="tools-descr">
              Редактор <br />
              кода
            </div>
          </div>
        </li>
        <li class="skills__list-item item5 list-item">
          <div class="list-item__wrap">
            <img src="@/assets/img/notion.svg" alt="notion" />
            <div class="tools-name">Notion</div>
            <div class="tools-descr">
              Project <br />
              managment
            </div>
          </div>
        </li>
        <li class="skills__list-item item6 list-item">
          <div class="list-item__wrap">
            <img src="@/assets/img/html.svg" alt="html" />
            <div class="tools-name">HTML5</div>
            <div class="tools-descr">
              Семантическая разметка кода <br />
              Использование БЭМ
            </div>
          </div>
        </li>
        <li class="skills__list-item item7 list-item">
          <div class="list-item__wrap">
            <img src="@/assets/img/sass.svg" alt="sass" />
            <div class="tools-name">SCSS</div>
            <div class="tools-descr">
              Стилизация элементов <br />
              на странице
            </div>
          </div>
        </li>
        <li class="skills__list-item item8 list-item">
          <div class="list-item__wrap">
            <img src="@/assets/img/JS.svg" alt="js" />
            <div class="tools-name">JavaScript</div>
            <div class="tools-descr">Скрипты для динамичности страницы</div>
          </div>
        </li>
      </ul>
    </div>
  </div>
</template>


<style lang="scss" scoped>
.skills {
  display: flex;

  &__list {
    display: grid;
    grid-template-columns: repeat(15, 1fr);
    grid-template-rows: repeat(6, 1fr);
    grid-column-gap: 10px;
    grid-row-gap: 10px;

    margin-bottom: 30px;
  }
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

      img {
        width: 60px;
      }

      .tools-name {
        margin-top: 15px;
        margin-bottom: 10px;
        color: #2e2e48;
        font: 500 16px/128% "Manrope", sans-serif;
      }
      .tools-descr {
        color: var(--gray-default, #79819a);
        font: 400 12px/128% "Manrope", sans-serif;
        letter-spacing: 0.101px;
      }
    }
  }
}

@media screen and (max-width: 1300px) {
  .skills {
    &__list {
      grid-template-columns: repeat(12, 1fr);
      grid-template-rows: repeat(12, 1fr);
    }

    .list-item {
      border-radius: 0;
    }

    .item6 {
      border-radius: 10px 0 0 0;
      grid-area: 1 / 1 / 5 / 5;
    }
    .item7 {
      grid-area: 1 / 5 / 5 / 9;
    }
    .item8 {
      border-radius: 0 10px 0 0;
      grid-area: 1 / 9 / 5 / 13;
    }
    .item4 {
      border-radius: 0 0 0 10px;
      grid-area: 5 / 1 / 9 / 5;
    }
    .item5 {
      grid-area: 5 / 5 / 9 / 9;
    }
    .item1 {
      border-radius: 0 0 10px 0;
      grid-area: 5 / 9 / 9 / 13;
    }
    .item2 {
      border-radius: 0 0 0 10px;
      grid-area: 9 / 3 / 13 / 7;
    }
    .item3 {
      border-radius: 0 0 10px 0;
      grid-area: 9 / 7 / 13 / 11;
    }
  }
}

@media screen and (max-width: 1100px) {
  .skills {
    &__list {
      grid-template-columns: repeat(6, 1fr);
      grid-template-rows: repeat(12, 1fr);
    }

    .list-item {
      border-radius: 0;
    }

    .item6 {
      border-radius: 10px 0 0 0;
      grid-area: 1 / 1 / 4 / 4;
    }
    .item7 {
      border-radius: 0 10px 0 0;
      grid-area: 1 / 4 / 4 / 7;
    }
    .item8 {
      grid-area: 4 / 1 / 7 / 4;
    }
    .item4 {
      grid-area: 4 / 4 / 7 / 7;
    }
    .item5 {
      grid-area: 7 / 1 / 10 / 4;
    }
    .item1 {
      grid-area: 7 / 4 / 10 / 7;
    }
    .item2 {
      border-radius: 0 0 0 10px;
      grid-area: 10 / 1 / 13 / 4;
    }
    .item3 {
      border-radius: 0 0 10px 0;
      grid-area: 10 / 4 / 13 / 7;
    }
  }
}

@media screen and (max-width: 500px) {
  .skills {
    .list-item {
      &__wrap {
        padding: 20px 10px;

        img {
          width: 40px;
        }

        .tools-descr {
          width: 80%;
        }
      }
    }
  }
}
</style>