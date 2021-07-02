<template>
  <q-page class="constrain q-pa-md">
    <div class="camera-frame q-pa-md">
      <img class="full-width" src="https://cdn.quasar.dev/img/parallax2.jpg" />
    </div>
  </q-page>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "PageCamera",
});
</script>

<style lang="scss">
.camera-frame {
  border: 2px solid $grey-10;
  border-radius: 10px;
}
</style>