<template>
	<div>
		{{ products }}
	</div>
</template>

<script>
import axios from "axios";

export default {
	async asyncData() {
		const response = await axios.get("http://localhost:3000/products");
		console.log("response: ", response);
		return {
			products: response.data,
		};
	},
};
</script>

<style>
</style>