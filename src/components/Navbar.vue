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
					<a href="" class="">Ana Sayfa</a>
				</li>
				<li class="inline-block mr-5 font-medium">
					<a href="">Ürünler</a>
				</li>
				<li class="inline-block mr-5 font-medium">
					<a href="" class="px-4 py-2 bg-pink-500 text-white rounded-3xl"
						>Modeller</a
					>
				</li>
				<li class="inline-block mr-5 font-medium">
					<a href="">Stok</a>
				</li>
			</ul>
			<UserCircleIcon class="inline-block mr-5 w-7 h-7 text-pink-500 hover:text-pink-700" />
			<Bars3Icon class="inline-block w-7 h-7 hover:text-pink-500 lg:hidden" />
		</div>
	</nav>
</template>

<script>
import { UserCircleIcon } from "@heroicons/vue/24/outline";
import { Bars3Icon } from "@heroicons/vue/24/outline";
export default {
    components:{UserCircleIcon, Bars3Icon},
	setup() {

		// const isActive = ref(false);
		return {UserCircleIcon, Bars3Icon};
	},
};
</script>
