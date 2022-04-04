<template>
    <p class="w-full font-mono font-extralight text-xs text-white">{{profileName}}</p>
</template>

<script lang="ts">
    import Vue from 'vue';

    export default Vue.extend({
        name: 'ProfileName',
        props: {
            profileName: {
                type: String
            }
        }
    })
</script>