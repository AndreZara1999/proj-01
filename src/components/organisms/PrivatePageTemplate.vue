<template>
    <div class="hidden md:flex w-full h-screen p-3 flex-row flex-nowrap bg-slate-800">
        <section 
            :class="{ 'w-[20%]': displayFullNavigation, 'w-[6%]': !displayFullNavigation }"
            class="p-5 mr-3 relative text-center shadow-lg bg-indigo-600 rounded-md"
        >
            <NavigationTools @toggleMenu="handleToggleMenu" :open="displayFullNavigation" />
            <NavigationContainer v-if="displayFullNavigation" />
            <SecondNavigationContainer v-else />
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
    import NavigationContainer from '@/components/molecules/NavigationContainer.vue';
    import SecondNavigationContainer from '@/components/molecules/SecondNavigationContainer.vue';
    import PageTitle from '@/components/atoms/PageTitle.vue';

    export default Vue.extend({
        name: 'PrivatePageTemplate',
        data() {
            return {
                displayFullNavigation: true
            };
        },
        props: {
            pageTitle: {
                type: String
            }
        },
        components: {
            NavigationTools,
            NavigationContainer,
            SecondNavigationContainer,
            PageTitle
        },
        methods: {
            handleToggleMenu() : void {
                this.displayFullNavigation = !this.displayFullNavigation;
            }
        }
    });
</script>