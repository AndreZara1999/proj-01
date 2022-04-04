<template>
    <h1 class="font-mono font-medium text-2xl text-white tracking-wide uppercase">{{pageTitle}}</h1>
</template>

<script lang="ts">
    import Vue from 'vue';

    export default Vue.extend({
        name: 'PageTitle',
        props: {
            pageTitle: {
                type: String
            }
        }
    });
</script>