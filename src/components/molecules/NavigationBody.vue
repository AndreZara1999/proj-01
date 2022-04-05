<template>
    <div class="w-full mt-3">
        <DasktopNavbar />
    </div>
</template>

<script lang="ts">
    import Vue from 'vue';

    // COMPONENTS
    import DasktopNavbar from '@/components/molecules/DesktopNavbar.vue';

    export default Vue.extend({
        name: 'NavigationBody',
        components: {
            DasktopNavbar
        }
    });
</script>