<template>
    <div class="w-full p-5 border border-solid border-transparent rounded-md shadow-lg">
        <slot></slot>
    </div>
</template>

<script lang="ts">
    import Vue from 'vue';

    export default Vue.extend({
        name: 'Card'
    });
</script>