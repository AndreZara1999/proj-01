<template>
    <div class="w-full py-2 px-3 text-center">
        <p class="font-mono font-thin text-xs">
            <slot></slot>
        </p>
    </div>
</template>

<script lang="ts">
    import Vue from 'vue';

    export default Vue.extend({
        name: 'CardFooter'
    })
</script>