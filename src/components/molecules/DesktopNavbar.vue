<template>
    <div class="w-full flex flex-col">
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