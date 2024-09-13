<script setup>
import { defineProps, toRefs } from 'vue'

const props = defineProps({
  numberDisplay: {
    type: String,
    default: '123123123123123'
  }
})

const { numberDisplay } = toRefs(props)

// function addToDisplay(text) {
//   numberDisplay.value = numberDisplay.value + text
//   return numberDisplay
// }
</script>

<template>
  <div class="numberDisplay">
    <input type="text" name="numberDisplay" :value="numberDisplay" readonly tabindex="-1" />
  </div>
</template>

<style scoped>
.numberDisplay {
  align-content: center;
  margin: 0 auto;
  width: 100%;
  position: relative;
}

.numberDisplay input[readonly] {
  outline: none;
  box-shadow: none;
  border: none;
  cursor: default;
  padding: 10px 20px;
  color: #333;
  background: #ccc;
}
</style>
