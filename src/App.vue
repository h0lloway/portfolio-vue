<script setup>
// import LayoutHeader from '@/components/layout/Header.vue';
import LayoutSidebar from "@/components/layout/Sidebar.vue";
import LayoutEducation from "@/components/layout/Education.vue";
import LayoutAchievements from "@/components/layout/Achievements.vue";
import LayoutSkills from "@/components/layout/Skills.vue";
import LayoutProjects from "@/components/layout/Projects.vue";
import LayoutCertificates from "@/components/layout/Certificates.vue";
import { ref } from "vue";

const isOpenMenu = ref(true);

const toggleMenu = () => {
  isOpenMenu.value = !isOpenMenu.value;
};
</script>

<template>
  <div class="container">
    <div class="sidebar-toggle" @click="toggleMenu">&#5125;</div>
    <!-- <layout-header/> -->
    <layout-sidebar :openSidebar="isOpenMenu" />

    <div :class="['content', { content_full: !isOpenMenu }]">
      <layout-education />
      <layout-achievements />
      <layout-skills />
      <layout-projects />
      <layout-certificates />
      <router-view />
    </div>
  </div>
</template>

<style lang="scss">
@import "./styles/global.scss";
@import "./styles/common.scss";
@import "./styles/sidebar.scss";

#app {
  padding: 0;
  font-family: "Outfit", Arial, Helvetica, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;

  text-align: left;
  max-width: 1400px;
  padding: 0 20px;
}

.content {
  position: relative;
  margin-left: 425px;
  padding: 30px;
  transition: 0.2s;
  &_full {
    margin-left: 0;
  }
}
.content::after {
  position: absolute;
  content: "";
  width: 2px;
  height: 96%;
  background: #e2e6ee;
  top: 35px;
  left: -36px;
}

@media screen and (max-width: 1560px) {
  .content {
    margin-left: 525px;
  }
}

@media screen and (max-width: 1023px) {
  .content {
    margin-left: 0;
  }

  .sidebar-toggle {
    position: fixed;
    left: 0;
    width: 15px;
    background: var(--primary-color);
    height: 100%;
    top: 0;
    z-index: 15;
    cursor: pointer;
    color: var(--white-color);
    display: flex;
    align-items: center;
    justify-content: center;
  }
}
</style>
