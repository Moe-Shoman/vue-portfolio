<template>
  <!-- Don't drop "q-app" class -->
  <div id="q-app">
      <!-- <img src="./assets/logo1.png" alt="Muhammad Shoman" class="logo"> -->
    <q-tabs slot="navigation" align="center">
      <q-tab slot="title" name="tab-1">Home</q-tab>
      <q-tab slot="title" name="tab-2">About</q-tab>
      <q-tab slot="title" name="tab-3">Projects</q-tab>
      <q-tab slot="title" name="tab-4">Contact</q-tab>
      <q-tab slot="title" name="tab-5">Blog</q-tab>
    </q-tabs>
      <router-view></router-view>
      <About/>
  </div>
</template>

<script>
/*
 * Root component
 */
import { QLayout, QToolbar, QBtn, QIcon, QTabs, QTab } from 'quasar'
import About from '@/About.vue'
export default {
  components: {
    About,
    QLayout,
    QToolbar,
    QBtn,
    QIcon,
    QTabs,
    QTab
  }
}
</script>

<style lang="stylus">
@import '~variables'

main
  text-align center;
  margin-top 40px;

.logo
  margin -5% auto;
  display block;
  width 25%;


</style>
