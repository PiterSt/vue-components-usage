<template>
	<div>
		<slot name="title"></slot>
		<span style="color: red"><slot name="subtitle">The subtitle</slot></span>
		<slot name="content"></slot>
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
	border: 1px solid rgb(206, 206, 206);
	text-align: center;
	max-width: 500px;
}


</style>