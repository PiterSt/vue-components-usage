<template>
	<div>
		<h2>Hypertrophy:</h2>
		<hr>
		<slot name="title"></slot>
		<span style="text-decoration: underline"><slot name="author">No author</slot></span>
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
	background-color:rosybrown;
}
</style>