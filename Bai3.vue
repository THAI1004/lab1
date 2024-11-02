<script setup>
import { ref } from 'vue'

const greeting = ref('Xin chào bạn! Chào mừng các bạn đến với Vue')
const buttonTitle = ref('Thay đổi lời chào')
const isGreetingChanged = ref(false)

const changeGreeting = e => {
  e.preventDefault()
  if (!isGreetingChanged.value) {
    greeting.value = 'Hello, World!'
    buttonTitle.value = 'Lời chào mới đã được cập nhật'
    isGreetingChanged.value = true
    alert(buttonTitle.value)
  } else {
    greeting.value = 'Xin chào bạn! Chào mừng các bạn đến với Vue'
    buttonTitle.value = 'Quay lại thành công'
    isGreetingChanged.value = false
    alert(buttonTitle.value)
  }
}
</script>

<template>
  <h1>{{ greeting }}</h1>
  <button :title="buttonTitle" @click="changeGreeting">
    {{ isGreetingChanged ? 'Click để quay lại' : 'Click để thay đổi' }}
  </button>
</template>
