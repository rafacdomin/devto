<template>
  <q-page class="row items-center justify-evenly">
    <div class="row">
      <h5 class="text-bold">Posts</h5>

      <div v-for="post in postCategories" :key="post">
        <q-btn
          no-caps
          text-color="dark"
          style="font-size: 16px"
          class="categorieBtn text-weight-light q-mr-sm"
          flat
          >{{ post }}</q-btn
        >
      </div>
    </div>
  </q-page>
</template>

<script lang="ts">
import { Vue, Component } from 'vue-property-decorator';

@Component({})
export default class Home extends Vue {
  postCategories = ['Feed', 'Week', 'Month', 'Year', 'Infinity', 'Latest'];
}
</script>

<style lang="scss">
.categorieBtn {
  &:hover {
    color: $primary;
  }
}
</style>
