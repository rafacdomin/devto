<template>
  <div>
    <h5 class="text-weight-bold q-ma-none">
      DEV is a community of 487,300 amazing developers
    </h5>
    <p class="text-subtitle1">
      We're a place where coders share, stay up-to-date and grow their careers.
    </p>
    <q-btn
      unelevated
      no-caps
      label="Create new account"
      class="full-width q-py-xs text-weight-light"
      color="primary"
      style="font-size: 16px"
    />
    <q-btn
      unelevated
      no-caps
      label="Log in"
      class="full-width q-py-xs text-weight-light q-my-sm"
      text-color="primary"
      style="font-size: 16px"
    />
  </div>
</template>

<script lang="ts">
import { Vue, Component } from 'vue-property-decorator';

@Component
export default class About extends Vue {}
</script>
