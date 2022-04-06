<template>
    <div class="w-full">
        <NavigationHead />
        <NavigationBody />
        <div class="absolute bottom-[25px] right-[25px]">
            <NavigationFooter />
        </div>
    </div>
</template>

<script lang="ts">
    import Vue from 'vue';
    // COMPONENTS
    import NavigationHead from '@/components/molecules/NavigationHead.vue';
    import NavigationBody from '@/components/molecules/NavigationBody.vue';
    import NavigationFooter from '@/components/molecules/NavigationFooter.vue';

    export default Vue.extend({
        name: "NavigationContainer",
        components: {
            NavigationHead,
            NavigationBody,
            NavigationFooter
        }
    })
</script>