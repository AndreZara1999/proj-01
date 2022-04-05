<template>
    <div class="hidden md:flex w-full h-screen p-3 flex-row flex-nowrap bg-slate-800">
        <section class="w-[20%] p-5 mr-3 relative text-center shadow-lg bg-indigo-600 rounded-md">
            <NavigationTools />
            <NavigationHead />
            <NavigationBody />
            <div class="absolute bottom-[25px] right-[25px]">
                <NavigationFooter />
            </div>
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
    import NavigationTools from '@/components/molecules/NavigationTools.vue';
    import NavigationHead from '@/components/molecules/NavigationHead.vue';
    import NavigationBody from '@/components/molecules/NavigationBody.vue';
    import NavigationFooter from '@/components/molecules/NavigationFooter.vue';
    import PageTitle from '@/components/atoms/PageTitle.vue';

    export default Vue.extend({
        name: 'PrivatePageTemplate',
        data() {
            return {

            };
        },
        props: {
            pageTitle: {
                type: String
            }
        },
        components: {
            NavigationTools,
            NavigationHead,
            NavigationBody, 
            NavigationFooter,
            PageTitle
        },
        methods: {
            toggleMenu() : void {

            }
        }
    });
</script>