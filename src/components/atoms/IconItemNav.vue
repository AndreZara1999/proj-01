<template>
    <router-link 
        :to='path'
        class="w-full mb-2 p-1 cursor-pointer hover:bg-slate-700 rounded-full"
    >
        <v-icon color="#FFFF">{{icon}}</v-icon>
    </router-link>
</template>

<script lang="ts">
    import Vue from 'vue';

    export default Vue.extend({
        name: 'IconItemNav',
        props: {
            path: {
                type: String,
                required: true
            },
            icon: {
                type: String,
                required: true
            }
        }
    });
</script>