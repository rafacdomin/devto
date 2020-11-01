<template>
  <q-layout view="hHh lpR fFf">
    <q-header bordered class="bg-white row items-center" style="height: 55px">
      <q-toolbar>
        <Header />
      </q-toolbar>
    </q-header>

    <q-page-container class="bg-secondary">
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script lang="ts">
import { Vue, Component } from 'vue-property-decorator';
import Header from '../components/Header.vue';

@Component({
  components: {
    Header,
  },
})
export default class MainLayout extends Vue {}
</script>

<style lang="scss" scoped>
.text-subtitle1 {
  color: $info;
  line-height: 24px;
}
</style>
