<template>
    <div class="w-full p-3">
        <h1 class="font-mono font-bold text-xl uppercase">
            <slot></slot>
        </h1>
    </div>    
</template>

<script lang="ts">
    import Vue from 'vue';

    export default Vue.extend({
        name: 'CardTitle'
    });
</script>