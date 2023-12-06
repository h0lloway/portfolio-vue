<script setup>
import { ref } from "vue";

const props = defineProps({
  openSidebar: {
    type: Boolean,
    required: false,
  },
});

// const links = ref([
//   { name: "Typography", href: "/typography" },
//   { name: "Button", href: "/button" },
// ]);
</script>


<template>
  <div :class="['sidebar', { sidebar_isopen: openSidebar }]">
    <!-- <router-link
      class="sidebar__link"
      v-for="link in links"
      :key="link.name"
      :to="link.href"
      >{{ link.name }}
      </router-link> -->

    <div class="sidebar__img">
      <img src="@/assets/img/me-squ.png" alt="##" />
    </div>

    <div class="sidebar__name">Anurag Yadav</div>

    <div class="sidebar__descr">
      A well-organized, creative and goaloriented graduate possessing excellent
      communication, problem-solving and leadership skills with a flair to
      explore Computer Science Engineering
    </div>

    <!-- контакты -->

    <ul class="sidebar__contact-list contact-list list-reset">
      <li class="contact-list__item common-link">
        <div class="common-link__wrap">
          <div class="img">
            <img src="@/assets/img/email.svg" alt="##" />
          </div>
          <div class="common-link__content">
            <span class="name">Email</span>
            <span class="descr">
              <a href="mailto:gvodb27@gmail.com">gvodb27@gmail.com</a>
            </span>
          </div>
        </div>
      </li>
      <li class="contact-list__item common-link">
        <div class="common-link__wrap">
          <div class="img">
            <img src="@/assets/img/website.svg" alt="##" />
          </div>
          <div class="common-link__content">
            <span class="name">Website</span>
            <span class="descr">
              <a href="https://h0lloway.github.io/my-portfolio/" target="_blank"
                >h0lloway.github.io/my-portfolio/</a
              >
            </span>
          </div>
        </div>
      </li>
      <li class="contact-list__item common-link">
        <div class="common-link__wrap">
          <div class="img">
            <img src="@/assets/img/phone.svg" alt="##" />
          </div>
          <div class="common-link__content">
            <span class="name">Phone</span>
            <span class="descr">
              <a href="tel:+79892804919">+7 (989) 280 49-19</a>
            </span>
          </div>
        </div>
      </li>
      <li class="contact-list__item common-link">
        <div class="common-link__wrap">
          <div class="img">
            <img src="@/assets/img/address.svg" alt="##" />
          </div>
          <div class="common-link__content">
            <span class="name">Address</span>
            <span class="descr">Aksai, Rostov-on-Don Region</span>
          </div>
        </div>
      </li>
    </ul>

    <!-- соц.сети -->

    <h5 class="sidebar__heading heading-5">Socials</h5>
    <ul class="sidebar__social-list social-list list-reset">
      <li class="social-list__item common-link">
        <div class="common-link__wrap">
          <div class="img">
            <img src="@/assets/img/inst.svg" alt="##" />
          </div>
          <div class="common-link__content">
            <span class="name">Instagram</span>
            <span class="descr">
              <a href="instagram.com/mksm.17" target="_blank">@mksm.17</a>
            </span>
          </div>
        </div>
      </li>
      <li class="social-list__item common-link">
        <div class="common-link__wrap">
          <div class="img">
            <img src="@/assets/img/github.svg" alt="##" />
          </div>
          <div class="common-link__content">
            <span class="name">Github</span>
            <span class="descr">
              <a href="https://github.com/h0lloway" target="_blank"
                >@h0lloway</a
              >
            </span>
          </div>
        </div>
      </li>
      <li class="social-list__item common-link">
        <div class="common-link__wrap">
          <div class="img">
            <img src="@/assets/img/vk.svg" width="30" alt="##" />
          </div>
          <div class="common-link__content">
            <span class="name">VK</span>
            <span class="descr">
              <a href="https://vk.com/h0lloway">@h0lloway</a>
            </span>
          </div>
        </div>
      </li>
      <!-- <li class="social-list__item common-link">
        <div class="common-link__wrap">
          <div class="img">
            <img src="@/assets/img/linked1.svg" width="30" alt="##" />
          </div>
          <div class="common-link__content">
            <span class="name">Linkedin</span>
            <span class="descr">
              <a href="https://vk.com/h0lloway">@anuragyadav</a>
            </span>
          </div>
        </div>
      </li> -->
    </ul>

    <!-- языки -->

    <h5 class="sidebar__heading heading-5">Languages</h5>
    <ul class="sidebar__lang-list lang-list list-reset">
      <li class="lang-list__item common-link">
        <div class="common-link__wrap">
          <div class="img">
            <img src="@/assets/img/india.svg" alt="##" />
          </div>
          <div class="common-link__content">
            <span class="name">Hindi</span>
            <span class="descr"> Native </span>
          </div>
        </div>
      </li>
      <li class="lang-list__item common-link">
        <div class="common-link__wrap">
          <div class="img">
            <img src="@/assets/img/eng.svg" alt="##" />
          </div>
          <div class="common-link__content">
            <span class="name">English</span>
            <span class="descr"> Professional working </span>
          </div>
        </div>
      </li>
      <li class="lang-list__item common-link">
        <div class="common-link__wrap">
          <div class="img">
            <img src="@/assets/img/spanish.svg" alt="##" />
          </div>
          <div class="common-link__content">
            <span class="name">Spanish</span>
            <span class="descr"> Elementary </span>
          </div>
        </div>
      </li>
    </ul>

    <!-- хобби и увлечения -->

    <h5 class="sidebar__heading heading-5">Hobby & Interests</h5>
    <ul class="sidebar__hobby-list hobby-list list-reset">
      <li class="hobby-list__item common-link">
        <div class="common-link__wrap">
          <div class="img">
            <img src="@/assets/img/game.svg" alt="##" />
          </div>
          <div class="common-link__content">
            <span class="descr">Gaming</span>
          </div>
        </div>
      </li>
      <li class="hobby-list__item common-link">
        <div class="common-link__wrap">
          <div class="img">
            <img src="@/assets/img/earth.svg" alt="##" />
          </div>
          <div class="common-link__content">
            <span class="descr">Travelling</span>
          </div>
        </div>
      </li>
      <li class="hobby-list__item common-link">
        <div class="common-link__wrap">
          <div class="img">
            <img src="@/assets/img/brush.svg" alt="##" />
          </div>
          <div class="common-link__content">
            <span class="descr">Sketching/Graffitti</span>
          </div>
        </div>
      </li>
      <li class="hobby-list__item common-link">
        <div class="common-link__wrap">
          <div class="img">
            <img src="@/assets/img/blog.svg" alt="##" />
          </div>
          <div class="common-link__content">
            <span class="descr">Blogging</span>
          </div>
        </div>
      </li>
    </ul>
  </div>
</template>