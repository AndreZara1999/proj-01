<template>
  <PrivatePageTemplate>
    <p>Hello</p>
  </PrivatePageTemplate>

  <!-- <Navbar /> -->
</template>

<script lang="ts">
  import Vue from 'vue'
  // COMPONENTS
  // import Navbar from '@/components/organisms/Navbar.vue';
  import PrivatePageTemplate from '@/components/organisms/PrivatePageTemplate.vue';

  export default Vue.extend({
    name: 'HomeViewasdasd',
    components: {
      // Navbar,
      PrivatePageTemplate
    }
  })
</script>
