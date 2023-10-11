<template>
	<div class="flex flex-col w-4/5 mx-auto mt-2">
		<h1 class="font-medium text-2xl pb-2">{{ activeFilter }}</h1>
		<div class="pb-2 flex items-center">
			<button
				@click="changeCurrentFilter('Tüm Ürünler')"
				class="border-2 border-pink-500 px-2 py-2 mr-2 rounded-3xl text-pink-700 hover:bg-pink-500 hover:text-white"
			>
				Tüm Ürünler
			</button>
			<button
				@click="changeCurrentFilter('Yünler')"
				class="border-2 border-pink-500 px-4 py-2 mr-2 rounded-3xl text-pink-700"
			>
				Yünler
			</button>
			<button
				@click="changeCurrentFilter('Tığlar')"
				class="border-2 border-pink-500 px-4 py-2 mr-2 rounded-3xl text-pink-700"
			>
				Tığlar
			</button>
			<button
				@click="changeCurrentFilter('Modeller')"
				class="border-2 border-pink-500 px-4 py-2 mr-2 rounded-3xl text-pink-700"
			>
				Modeller
			</button>
		</div>
	</div>
</template>

<script>
import { ref } from 'vue';

export default {
	setup () {
		const activeFilter = ref('Tum Ürünler')

		const changeCurrentFilter = (value) => {
			activeFilter.value = value
		}

		return {activeFilter, changeCurrentFilter}
	}
}
</script>