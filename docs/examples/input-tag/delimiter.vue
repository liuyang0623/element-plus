<template>
  <el-input-tag
    v-model="input"
    draggable
    placeholder="Try to separate words with ,"
    :delimiter="reg"
  />
</template>

<script lang="ts" setup>
import { ref } from 'vue'
const input = ref<string[]>([])
const reg = /[\r\n,]/
</script>
