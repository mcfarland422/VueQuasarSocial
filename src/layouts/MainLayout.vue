<template>
  <q-layout view="lHh Lpr lFf">
    <q-header elevated>
      <q-toolbar class="constrain">
        <q-btn
          class="large-screen-only q-mr-sm"
          flat
          round
          color="white"
          size="18px"
          dense
          icon="eva-camera-outline"
          to="/camera"
        />
        <q-toolbar-title class="text-grand-hotel text-bold">
          Friend Zone
        </q-toolbar-title>
        <q-btn
          class="large-screen-only"
          flat
          round
          color="white"
          size="18px"
          dense
          icon="eva-home-outline"
          to="/"
        />
      </q-toolbar>
    </q-header>

    <q-footer class="bg-white small-screen-only" bordered>
      <q-tabs
        class="text-grey-10"
        active-color="primary"
        indicator-color="transparent"
      >
        <q-route-tab to="/" icon="eva-home-outline" />
        <q-route-tab to="/camera" icon="eva-camera-outline" />
      </q-tabs>
    </q-footer>

    <q-page-container class="bg-grey-1">
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>
import { defineComponent, ref } from "vue";

export default defineComponent({
  name: "MainLayout",

  setup() {
    return {};
  },
});
</script>

<style lang="scss">
.q-toolbar {
  @media (min-width: $breakpoint-sm-min) {
    height: 77px;
  }
}
.q-toolbar__title {
  font-size: 2rem;
  @media (max-width: $breakpoint-xs-max) {
    text-align: center;
  }
}
.q-footer {
  .q-tab__icon {
    font-size: 2.2rem;
    padding: 1rem;
  }
}
</style>