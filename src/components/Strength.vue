<template>
	<div>
		<h2>Strength</h2>
		<hr>
		<slot name="title"></slot>
		<span style="text-decoration: underline"><slot name="author">Unknown author</slot></span>
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
	background-image: linear-gradient(to bottom right, rgb(7, 7, 7), rgb(85, 85, 85));
	color: white;
}

</style>