/** MOBILE FIRST */
<template>
    <DesktopNavbar />
</template>

<script lang="ts">
    import Vue from 'vue';
    // COMPONENTS
    import DesktopNavbar from '@/components/molecules/DesktopNavbar.vue';

    export default Vue.extend({
        name: 'Navbar',
        components: {
            DesktopNavbar
        }
    });
</script>