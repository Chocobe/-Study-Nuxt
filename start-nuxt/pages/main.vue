<template>
	<div>
		<p>Nuxt 메인 페이지 입니다.</p>

		<ProductList />
	</div>
</template>

<script>
import axios from "axios";
import ProductList from "~/components/ProductList.vue";

export default {
	components: {
		ProductList,
	},

	// async asyncData() {
	// 	const response = await axios.get("http://localhost:3000/products");
	// 	console.log("response: ", response);
	// 	return {
	// 		products: response.data,
	// 	};
	// },
};
</script>

<style scoped>
/*  */
</style>