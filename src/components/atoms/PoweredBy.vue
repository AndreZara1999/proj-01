<template>
    <p class="font-sans text-white text-[10px] font-normal">Powered by: {{text}}</p>
</template>

<script lang="ts">
    import Vue from 'vue';

    export default Vue.extend({
        name: "PoweredBy",
        props: {
            text: {
                type: String,
                default: 'Zarantonello Andrea'
            }
        }
    });
</script>