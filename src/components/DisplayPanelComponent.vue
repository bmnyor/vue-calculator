<script setup>

import { defineProps, toRefs  } from 'vue'

const props= defineProps({
  numberDisplay: {
    type: String,
    default: ""
  }
})

const { numberDisplay } = toRefs(props)

</script>

<template>
	<div class="numberDisplay">
		<input type="text" name="numberDisplay" :value="numberDisplay" readonly tabindex="-1" style="height: 30px;width: 30vw;">
	</div>
</template>

<style scoped>
input[readonly] {
  outline: none;
  box-shadow: none;
}
</style>
