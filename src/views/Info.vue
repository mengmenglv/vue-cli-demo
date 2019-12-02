<template>
    <div>
        this is info
        <button type="button" @click="add()"></button>
    </div>
</template>

<script>
    import store from '@/store/index'

    export default {
        name: "Info",
        store,
        methods: {
            add () {
               console.log('add info');
               store.commit('increase')
            }
        }
    }
</script>

<style scoped>

</style>