<template>
    <div class="w-48 rounded-full">
        <!-- <div v-html="svgAvatar"></div> -->
    </div>
</template>

<script lang="ts">
    import Vue from 'vue';

    import { createAvatar } from '@dicebear/avatars';
    // import * as style from '@dicebear/avatars-identicon-sprites';
    new Vue({
        name: "Avatar",
        data() {
            return {
                svgAvatar: ''
            };
        },
        methods: {
            createAvatar() : void {
                console.log('Hello');
                // this.svgAvatar = createAvatar(style, {
                //     seed: 'custom-seed',
                //     // ... and other options
                // });
            }
        },
        mounted() {
            this.createAvatar();
        }        
    });
</script>