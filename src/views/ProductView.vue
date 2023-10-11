<template>
	<div class="flex flex-col">
		<Filter />
		<div class="mt-2 w-4/5 mx-auto h-screen">
			<div
				class="grid grid-cols-1 gap-4 justify-items-center overflow-y-auto h-screen sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-5 lg:w-full lg:content-start"
			>
				<div
					class="w-[250px] h-[350px] backdrop-blur-xl bg-white/30 shadow-lg rounded-md"
					v-for="item in items"
					:key="item.id"
				>
					<ProductCard :data="item"/>
				</div>
			</div>
		</div>
	</div>
</template>

<script>
import { ref } from "vue";
import Filter from "../components/Filter.vue";
import ProductCard from "../components/ProductCard.vue";
import { products } from "../data/product.js";

export default {
	components: { Filter, ProductCard },
	setup() {
		const items = ref(products);
		return { Filter, ProductCard, items };
	},
};
</script>
