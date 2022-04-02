<template>
    <div class="w-full px-3 py-2">
        <slot></slot>
    </div>
</template>

<script lang="ts">
    import Vue from 'vue';

    export default Vue.extend({
        name: 'CardBody'
    });
</script>