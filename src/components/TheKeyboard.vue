<script setup>
import { ref } from 'vue'
import BackSpace from './icons/BackSpace.vue'
import MathDivide from './icons/MathDivide.vue'
// import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome'

const test = ref('')

// function addText(text) {}
</script>

<template>
  <div class="btn-container mt-5">
    {{ test }}
    <button @click="addNumber()">%</button>
    <button @click="addNumber()">CE</button>
    <button @click="addNumber()">C</button>
    <button>
      <MathDivide />
    </button>
    <button @click="addNumber()">7</button>
    <button @click="addNumber()">8</button>
    <button @click="addNumber()">9</button>
    <button @click="addNumber()">*</button>
    <button @click="addNumber()">4</button>
    <button @click="addNumber()">5</button>
    <button @click="addNumber()">6</button>
    <button>-</button>
    <button @click="addNumber()">1</button>
    <button @click="addNumber()">2</button>
    <button @click="addNumber()">3</button>
    <button>+</button>
    <button class="backspace">
      <BackSpace />
    </button>
    <button @click="addNumber()">0</button>
    <button @click="addNumber()">.</button>
    <button>=</button>
  </div>
</template>

<style>
.mt-5 {
  margin-top: 2rem;
}

.btn-container {
  display: inline-grid;
  grid-template-columns: repeat(4, 1fr);
  grid-column-gap: 2px;
  grid-row-gap: 2px;
  justify-items: center;
  justify-content: center;
  align-items: center;
}

.btn-container :nth-child(1) {
  border-top-left-radius: 10px;
}
.btn-container :nth-child(4) {
  border-top-right-radius: 10px;
}
.btn-container :nth-child(17) {
  border-bottom-left-radius: 10px;
}
.btn-container :nth-child(20) {
  border-bottom-right-radius: 10px;
}

.backspace {
  background-color: #794833;
}

button {
  border: none;
  min-width: 60px;
  max-width: 60px;
  height: 80px;
  background-color: #4c3c3c;
}
</style>
