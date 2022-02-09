

<template>
    <h1>这是首页</h1>
    <Todolist></Todolist>    
    <div @click="add">
        {{count}}
    </div>
</template>

<script setup>
import Todolist from '../components/Todolist.vue'
import { computed } from 'vue'
import {useStore} from 'vuex'
let store = useStore()
let count = computed(()=>store.state.count)

function add(){
    store.commit('add')
}
</script>   
