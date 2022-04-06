<template>
    <div class="w-full p-2 pt-0 text-right">
        <v-icon
          dark
          left
          :class="{ 'rotate-180' : !open }"
          class="!m-0 cursor-pointer"
          v-on:click="handleClick"
        >mdi-arrow-left</v-icon>
    </div>
</template>

<script lang="ts">
    import Vue from 'vue';

    export default Vue.extend({
        name: 'NavigationTools',
        props: {
            open: {
                type: Boolean,
                required: true   
            }
        },
        methods: {
            handleClick: function () {
                this.$emit('toggleMenu', null)
            }
        }
    });
</script>