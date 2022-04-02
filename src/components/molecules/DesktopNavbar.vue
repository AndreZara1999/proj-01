<template>
    <div class="w-full hidden sm:hidden lg:flex flex-row flex-nowrap bg-sky-600">
        <ItemNav path='/' text="Home" />
        <ItemNav path='/about' text="About" />
    </div>
</template>

<script lang="ts">
    import Vue from 'vue';
    // COMPONENTS
    import ItemNav from '@/components/atoms/ItemNav.vue';
    
    export default Vue.extend({
        name: 'DesktopNavbar',
        components: {
            ItemNav
        }
    })
</script>