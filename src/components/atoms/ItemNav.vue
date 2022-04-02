<template>
    <div class="w-fill py-1 my-2 mx-2 font-mono font-normal text-xs">
        <router-link :to='path'>{{text}}</router-link>
    </div>
</template>

<script lang="ts">
    import Vue from 'vue';

    export default Vue.extend({
        name: 'ItemNav',
        props: {
            path: {
                type: String,
                required: true
            }, 
            text: {
                type: String,
                required: true
            }
        }

    });
</script>