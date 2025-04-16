<script setup lang="ts">
import DarkModeToggle from "./components/DarkModeToggle.vue";
import PageFooter from "./components/PageFooter.vue";
import PageHeader from "./components/PageHeader.vue";
import SectionTitle from "./components/SectionTitle.vue";
import Motivation from "./views/Motivation.vue";
import Profile from "./views/Profile.vue";
import Projects from "./views/Projects.vue";
</script>

<template>
  <DarkModeToggle />
  <PageHeader
    title="Víctor Olea"
    subtitle="Mechatronics Enginner & Maker Developer"
  />
  <SectionTitle title="Profile" />
  <Profile />
  <SectionTitle title="Projects" />
  <Projects />
  <SectionTitle title="Motivation" />
  <Motivation />
  <PageFooter />
</template>
