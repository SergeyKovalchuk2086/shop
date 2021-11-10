<template>
	<div class="v-catalog-item">
		<img class="v-catalog-item_img" :src="require('../assets/images/' + product_data.image)" alt="img" />
		<p class="v-catalog-item__name">{{ product_data.name }}</p>
		<p class="v-catalog-item__price">Price : {{ product_data.price }} р.</p>
		<button class="v-catalog-item__btn btn">Add to cart</button>
	</div>
</template>

<script>
export default {
	name: "v-catalog-item",
	props: {
		product_data: {
			type: Object,
			default() {
				return {};
			},
		},
	},
};
</script>

<style scoped>
.v-catalog-item {
	flex-basis: 25%;
	box-shadow: 0 0 8px 0 #e0e0e0;
	padding: 16px;
	margin-bottom: 16px;
}

.v-catalog-item_img {
   width: 150px;
}
</style>
