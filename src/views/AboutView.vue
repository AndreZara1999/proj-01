<template>
  <PrivatePageTemplate pageTitle='About'>
    <p>About page</p>
  </PrivatePageTemplate>
</template>

<script lang="ts">
  import Vue from 'vue';
  // COMPONENTS
  import PrivatePageTemplate from '@/components/organisms/PrivatePageTemplate.vue';

  export default Vue.extend({
    components: {
      PrivatePageTemplate
    }
  })
</script>
