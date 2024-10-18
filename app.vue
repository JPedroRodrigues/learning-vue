<template>
    <main class="grid grid-cols-4 gap-0">
        <div class="col-span-1">
            <SideBar />
        </div>
        <div class="col-span-3">
            <Forms />
        </div>
    </main>
</template>

<script>
    import { defineComponent } from 'vue';
    import SideBar from './components/SideBar.vue';
    import Forms from './components/Forms.vue';

    export default defineComponent({
        name: "App",
        components: {
            SideBar,
            Forms
        }
    })
</script>