<template>
    <div class="w-full mt-3 flex flex-col">
        <IconItemNav path='/' icon="mdi-home" />
        <IconItemNav path='/about' icon="mdi-domain" />
    </div>
</template>

<script lang="ts">
    import Vue from 'vue';
    // COMPONENTS
    import IconItemNav from '@/components/atoms/IconItemNav.vue';

    export default Vue.extend({
        name: 'SecondNavigationContainer',
        components: {
            IconItemNav
        }
    });
</script>