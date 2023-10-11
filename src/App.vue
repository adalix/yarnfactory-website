<template>
	<div
		class="bg-[url('/src/assets/img/bg.jpg')] bg-fixed bg-no-repeat bg-cover overflow-hidden sm:bg-center "
	>
		<div class="flex flex-col pt-5 h-screen">
			<Navbar />
			<RouterView />
		</div>
	</div>
</template>

<script>
import Navbar from "./components/Navbar.vue";
import { RouterView } from "vue-router";

export default {
	components: { Navbar },

	setup() {
		return { Navbar };
	},
};
</script>
