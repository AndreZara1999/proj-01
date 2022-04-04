<template>
    <div class="hidden md:flex w-full h-screen p-3 flex-row flex-nowrap bg-slate-800">
        <section class="md:w-1/6 lg:w-1/4 xl:w-1/5 2xl:w-1/6 2xl:max-w-xs p-5 md:mr-1 lg:mr-5 xl:mr-10 shadow-lg bg-indigo-600 rounded-md">
            <NavigationHead />
        </section>
        <section class="w-full p-5 shadow-lg bg-slate-700 rounded-md">
            <PageTitle :pageTitle="pageTitle" />
            <slot></slot>
        </section>
    </div>
</template>

<script lang="ts">
    import Vue from 'vue';
    // COMPONENTS
    import NavigationHead from '@/components/molecules/NavigationHead.vue';
    import PageTitle from '@/components/atoms/PageTitle.vue';

    export default Vue.extend({
        name: 'PrivatePageTemplate',
        props: {
            pageTitle: {
                type: String
            }
        },
        components: {
            NavigationHead,
            PageTitle
        }
    });
</script>