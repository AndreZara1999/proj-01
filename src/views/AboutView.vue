<template>
  <div>
    <ItemNav path='/' text="Home"/>
    <div class="about">
      <h1>This is an about page</h1>
    </div>
  </div>
</template>

<script lang="ts">
  import Vue from 'vue';
  // COMPONENTS
  import ItemNav from '@/components/organisms/Navbar.vue';

  export default Vue.extend({
    components: {
      ItemNav
    }
  })
</script>
