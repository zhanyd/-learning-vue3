
<template>
    <h1>这是关于页面</h1>
    <Rate :value="score"></Rate>
    <Rate value="3.5" theme="red">课程评分</Rate>
    <Rate value="5" theme="black"></Rate>
</template>

<script setup>
import { ref } from 'vue'
import Rate from '../components/Rate.vue'

let score = ref(3)
</script>
