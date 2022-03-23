<template>
  <div>Hello, {{ name }}!</div>
  <Form v-model="name" @submit="submitForm" />
</template>

<script setup>
import { ref } from 'vue'
import Form from './components/Form.vue'

const name = ref('')

function submitForm() {
  console.log(name.value)
}
</script>