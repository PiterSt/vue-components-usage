<template>
    <div class="container">
        <div class="row">
            <div class="col-xs-12">
				<h1>Hello world!</h1>
				<quote/>
            </div>
        </div>
    </div>
</template>

<script>
    import Quote from './components/Quote.vue'

    export default {
		components: {
			Quote
		}
    }
</script>

<style scoped>
div {
	margin: 0 auto;
	text-align: center;
}
</style>
