<template>
	<div class="card-image">
		<img
			class="w-[250px] h-[270px] mx-auto rounded-t-lg"
			:src="data.image"
			alt=""
		/>
	</div>
	<div class="card-content pt-2 px-3">
		<div class="text-gray-900 text-xl font-bold pb-2">
			<h2>{{data.brand}} <span>{{data.detail.model}}</span></h2>
		</div>
		<div class="text-gray-900">
			<span class="mr-5" v-if="data.category === 'Yun'">Renk: {{data.detail.colorCode}}</span>
            <span class="mr-5" v-else>No: {{data.detail.no}}</span>
			<span>Stok: {{ data.stockCount }}</span>
		</div>
	</div>
</template>

<script>
// import { ref } from 'vue';

export default {
    props:{
        data: Object,
    },
	setup() {
		return {};
	},
};
</script>
