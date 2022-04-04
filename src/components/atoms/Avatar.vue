<template>
    <div class="w-[3rem] mx-auto rounded-full" v-html="svgAvatar"></div>
</template>

<script lang="ts">
    import Vue from 'vue';

    import { createAvatar } from '@dicebear/avatars';
    import * as style from '@dicebear/avatars-identicon-sprites';

    export default Vue.extend({
        name: "Avatar",
        data() {
            return {
                svgAvatar: ''
            };
        },
        methods: {
            createAvatar() : void {
                this.svgAvatar = createAvatar(style, {
                    seed: 'custom-seed',
                    // ... and other options
                });
            }
        },
        mounted() {
            this.createAvatar();
        }        
    });
</script>