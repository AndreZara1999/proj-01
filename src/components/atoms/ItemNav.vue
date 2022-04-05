<template>
    <router-link 
        :to='path' 
        class="w-fill p-1 mt-1 text-center font-mono font-semibold text-white text-xs uppercase rounded-full bg-slate-800"
    >{{text}}</router-link>
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