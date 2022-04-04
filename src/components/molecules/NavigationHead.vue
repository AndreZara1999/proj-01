<template>
    <div class="w-full text-center">
        <!-- Avatar component -->
        <Avatar></Avatar>
        <!-- Profile Name -->

    </div>
</template>

<script lang="ts">
    import Vue from 'vue';
    // COMPONENENTS
    import Avatar from '@/components/atoms/Avatar.vue';

    export default Vue.extend({
        name: 'NavigationHead',
        components: {
            Avatar
        }
    });
</script>