<template>
	<div class="v-main-wrapper">
		<vCatalog />
		<vCart />
	</div>
</template>

<script>
import vCatalog from "@/components/v-catalog";
import vCart from "@/components/v-cart";

export default {
	name: "v-main-wrapper",
	components: { vCatalog, vCart },

	props: {},
	data() {
		return {};
	},

	computed: {},
	methods: {},
	watch: {},
};
</script>

<style scoped>
.v-main-wrapper {
	max-width: 900px;
	margin: 0 auto;
}
</style>
