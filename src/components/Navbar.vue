<template>
	<nav
		class="w-4/5 h-11 flex items-center justify-between mx-auto py-8 backdrop-blur-xl bg-white/30 rounded-full shadow-md"
	>
		<h2 class="mx-12 text-2xl font-bold cursor-pointer">
			Yarn<span class="text-pink-500">Factory</span>
		</h2>

		<div class="flex items-center justify-evenly mx-12">
			<ul class="hidden sm:hidden md:hidden lg:block">
				<li class="inline-block mr-5 font-medium">
					<RouterLink
						to="/"
						class="px-4 py-2 hover:bg-pink-500 hover:text-white hover:rounded-3xl"
						>Ana Sayfa</RouterLink
					>
				</li>
				<li class="inline-block mr-5 font-medium">
					<RouterLink
						to="/product"
						class="px-4 py-2 hover:bg-pink-500 hover:text-white hover:rounded-3xl"
						>Ürünler</RouterLink
					>
				</li>
				<li class="inline-block mr-5 font-medium">
					<RouterLink
						to="/"
						class="px-4 py-2 hover:bg-pink-500 hover:text-white hover:rounded-3xl"
						>Modeller</RouterLink
					>
				</li>
				<li class="inline-block mr-5 font-medium">
					<RouterLink
						to="/product"
						class="px-4 py-2 hover:bg-pink-500 hover:text-white hover:rounded-3xl"
						>Stok</RouterLink
					>
				</li>
			</ul>
			<UserIcon class="inline-block mr-5 w-6 h-6 text-pink-500 fill-pink-500" />
			<Bars3Icon class="inline-block w-6 h-6 hover:text-pink-500 lg:hidden" />
		</div>
	</nav>
</template>

<script>
import { UserIcon } from "@heroicons/vue/24/outline";
import { Bars3Icon } from "@heroicons/vue/24/outline";
import { RouterLink } from "vue-router";
export default {
	components: { UserIcon, Bars3Icon },
	setup() {
		return { UserIcon, Bars3Icon };
	},
};
</script>
