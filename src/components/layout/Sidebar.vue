<script setup>
import { ref } from "vue";

const props = defineProps({
  openSidebar: {
    type: Boolean,
    required: false,
  },
});
</script>


<template>
  <div :class="['sidebar', { sidebar_isopen: openSidebar }]">

    <div class="sidebar__img">
      <img src="@/assets/img/me-squ.png" alt="my photo" />
    </div>

    <div class="sidebar__name">Dubrovin Maksim</div>

    <div class="sidebar__descr">
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Quo sequi facilis
      nostrum, culpa, dignissimos dicta aliquid ut commodi aspernatur harum
      voluptatum enim libero.
    </div>

    <!-- контакты -->

    <ul class="sidebar__contact-list contact-list list-reset">
      <li class="contact-list__item common-link">
        <div class="common-link__wrap">
          <div class="img">
            <img src="@/assets/img/email.svg" alt="email" />
          </div>
          <div class="common-link__content">
            <span class="name">Email</span>
            <span class="descr">
              <a href="mailto:gvozdb27@gmail.com">gvozdb27@gmail.com</a>
            </span>
          </div>
        </div>
      </li>
      <li class="contact-list__item common-link">
        <div class="common-link__wrap">
          <div class="img">
            <img src="@/assets/img/website.svg" alt="website" />
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
            <img src="@/assets/img/phone.svg" alt="phone" />
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
            <img src="@/assets/img/address.svg" alt="address" />
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
            <img src="@/assets/img/inst.svg" alt="inst" />
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
            <img src="@/assets/img/github.svg" alt="github" />
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
            <img src="@/assets/img/vk.svg" width="30" alt="vk" />
          </div>
          <div class="common-link__content">
            <span class="name">VK</span>
            <span class="descr">
              <a href="https://vk.com/h0lloway" target="_blank">@h0lloway</a>
            </span>
          </div>
        </div>
      </li>
    </ul>

    <!-- языки -->

    <h5 class="sidebar__heading heading-5">Languages</h5>
    <ul class="sidebar__lang-list lang-list list-reset">
      <li class="lang-list__item common-link">
        <div class="common-link__wrap">
          <div class="img">
            <img src="@/assets/img/rus.svg" width="34" alt="ru" />
          </div>
          <div class="common-link__content">
            <span class="name">Russian</span>
            <span class="descr"> Native </span>
          </div>
        </div>
      </li>
      <li class="lang-list__item common-link">
        <div class="common-link__wrap">
          <div class="img">
            <img src="@/assets/img/eng.svg" alt="eng" />
          </div>
          <div class="common-link__content">
            <span class="name">English</span>
            <span class="descr"> Intermediate </span>
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
            <img src="@/assets/img/family.svg" alt="family" />
          </div>
          <div class="common-link__content">
            <span class="descr">Family/house</span>
          </div>
        </div>
      </li>
      <li class="hobby-list__item common-link">
        <div class="common-link__wrap">
          <div class="img">
            <img src="@/assets/img/computer.svg" alt="gaming" />
          </div>
          <div class="common-link__content">
            <span class="descr">Gaming</span>
          </div>
        </div>
      </li>
      <li class="hobby-list__item common-link">
        <div class="common-link__wrap">
          <div class="img">
            <img src="@/assets/img/tv.svg" alt="TV" />
          </div>
          <div class="common-link__content">
            <span class="descr">TV series</span>
          </div>
        </div>
      </li>
      <li class="hobby-list__item common-link">
        <div class="common-link__wrap">
          <div class="img">
            <img src="@/assets/img/fitness.svg" alt="fitness" />
          </div>
          <div class="common-link__content">
            <span class="descr">Fitness</span>
          </div>
        </div>
      </li>
    </ul>
  </div>
</template>