<template lang="">
    <div>
        Default Page
        <AppButton></AppButton>
        <h1>Hello, Nuxt!</h1>
        <div class="demo-color-block">
            <span class="demonstration">With no default value</span>
            <el-color-picker v-model="color" />
        </div>
        <label for="#title">{{ title }}</label>
        <input id='title' type="text" v-model="title">

        <!-- <HelloButton></HelloButton> -->
    </div>
</template>
<script setup lang="ts">
    const color = ref('')
    const title = ref('')

</script>
<style lang="scss">
    h1 {
    color: v-bind(color);
    }
</style>