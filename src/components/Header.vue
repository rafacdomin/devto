<template>
  <q-toolbar-title class="row items-center">
    <q-btn dense unelevated>
      <q-avatar rounded size="xl">
        <img src="../assets/logo-header.png" />
      </q-avatar>
    </q-btn>
    <q-input
      :dense="true"
      outlined
      v-model="search"
      placeholder="Search..."
      style="font-size: 16px"
      class="q-ml-sm col-4 gt-xs"
    />

    <q-input
      :dense="true"
      outlined
      v-model="search"
      placeholder="Search..."
      class="q-ml-sm col-7 lt-sm"
    />

    <q-btn
      unelevated
      no-caps
      label="Log in"
      class="text-weight-regular q-ml-auto gt-xs"
      style="font-size: 16px"
      text-color="primary"
    />
    <q-btn
      unelevated
      no-caps
      label="Create account"
      class="text-weight-regular q-ml-sm gt-xs"
      style="font-size: 16px"
      color="primary"
      text-color="white"
    />

    <!-- mobile menu -->
    <q-btn
      flat
      round
      dense
      icon="menu"
      class="q-ml-md black lt-sm q-ml-auto"
      style="color: #666"
    >
      <q-menu fit>
        <div class="q-pa-lg">
          <About />

          <hr />

          <q-btn
            unelevated
            no-caps
            flat
            color="primary"
            text-color="dark"
            label="About DEV"
            class="full-width q-mt-sm text-weight-light"
            align="left"
            style="font-size: 16px"
          />

          <q-btn
            unelevated
            no-caps
            flat
            color="primary"
            text-color="dark"
            label="Learn more"
            class="full-width q-my-sm text-weight-light"
            align="left"
            style="font-size: 16px"
          />
        </div>
      </q-menu>
    </q-btn>
  </q-toolbar-title>
</template>

<script lang="ts">
import { Vue, Component } from 'vue-property-decorator';
import About from './About.vue';

@Component({
  components: {
    About,
  },
})
export default class Header extends Vue {
  search = '';
}
</script>
