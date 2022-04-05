<template>
    <div class="w-full text-center">
        <PoweredBy />
    </div>
</template>

<script lang="ts">
    import Vue from 'vue';
    // COMPONENTS
    import PoweredBy from '@/components/atoms/PoweredBy.vue';

    export default Vue.extend({
        name: 'NavigationFooter',
        components: {
            PoweredBy
        }
    });
</script>