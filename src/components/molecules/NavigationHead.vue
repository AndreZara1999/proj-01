<template>
    <div class="w-full text-center">
        <Avatar></Avatar>
        <ProfileName class="mt-[10px]" :profileName="profileName" />
    </div>
</template>

<script lang="ts">
    import Vue from 'vue';
    // COMPONENENTS
    import Avatar from '@/components/atoms/Avatar.vue';
    import ProfileName from '@/components/atoms/ProfileName.vue';

    export default Vue.extend({
        name: 'NavigationHead',
        components: {
            Avatar,
            ProfileName
        },
        data() {
            return {
                profileName: '',
                avatarRef: ''
            };
        },
        methods: {
            fetchProfileData() : void {
                this.profileName = 'Zarantonello Andrea'
            }
        },
        mounted() {
            this.fetchProfileData();
        }
    });
</script>