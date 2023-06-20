<script setup lang="ts">
import { reactive, ref } from 'vue'
const labelPosition = ref('right')
const form = reactive({
  restaurantName: '',

})

</script>

<template>
  <main>
	<h2>Hello</h2>

	<el-form
		:model="form"
		label-width="120px"
		:label-position="labelPosition"
		>
		<el-form-item label="Nome do restaurante">
			<el-input v-model="form.restaurantName"></el-input>

		</el-form-item>
	</el-form>
  </main>
</template>
