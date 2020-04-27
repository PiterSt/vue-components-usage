<template>
	<div>
		<h2>New Quote:</h2>
		<slot name="title"></slot>
		<span style="color: grey; text-decoration: underline"><slot name="subtitle">The subtitle</slot></span>
		<slot name="content"></slot>
	</div>
</template>

<script>
export default {
	
}
</script>

<style scoped>

</style>