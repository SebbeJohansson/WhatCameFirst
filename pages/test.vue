<template>
  <div class="container">
    {{ $t('message') }}
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  nuxtI18n: {
    paths: {
      en: '/test',
      sv: '/svenskttest',
    }
  }
})
</script>

<style>
</style>
