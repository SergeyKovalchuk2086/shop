<template>
	<div class="v-catalog">
		<h1>Catalog</h1>
		<div class="v-catalog__list">
			<vCatalogItem
         v-for="product in products" :key="product.article" :product_data="product"
         />
		</div>
	</div>
</template>

<script>
import vCatalogItem from "@/components/v-catalog-item";
export default {
	name: "v-catalog",
	components: {
		vCatalogItem,
	},
	data() {
		return {
			products: [
				{
					image: "1.jpg",
					name: "Toyota",
					price: 2100,
					article: "T1",
					available: true,
					category: "Мужские",
				},
				{
					image: "2.jpg",
					name: "BMW",
					price: 3150,
					article: "T2",
					available: true,
					category: "Женские",
				},
				{
					image: "3.jpg",
					name: "Mercedes-Benz",
					price: 4200,
					article: "T3",
					available: false,
					category: "Женские",
				},
				{
					image: "4.jpg",
					name: "Bugatti",
					price: 5300,
					article: "T4",
					available: true,
					category: "Мужские",
				},
				{
					image: "5.jpg",
					name: "Lamborghini",
					price: 6500,
					article: "T5",
					available: false,
					category: "Женские",
				},
				{
					image: "6.jpg",
					name: "Bugatti",
					price: 8700,
					article: "T6",
					available: true,
					category: "Женские",
				},
			],
		};
	},
};
</script>

<style scoped>
.v-catalog__list {
	display: flex;
	flex-wrap: wrap;
	justify-content: space-between;
	align-items: center;
}
</style>
