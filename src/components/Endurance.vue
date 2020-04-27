<template>
	<div>
		<h2>Endurance</h2>
		<hr>
		<slot name="title"></slot>
		<span style="text-decoration: underline"><slot name="author">Author who knows</slot></span>
		<slot name="duration"></slot>
	</div>
</template>

<script>
export default {
	
}
</script>

<style scoped>
div {
	margin: 40px auto;
	padding: 60px;
	box-shadow: 7px 7px 15px rgb(97, 97, 97);
	text-align: center;
	max-width: 500px;
	background-image: linear-gradient(to bottom right, rgb(201, 1, 1), rgb(255, 57, 57));
	color: white;
}
</style>