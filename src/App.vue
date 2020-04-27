<template>
    <div class="container">
        <div class="row">
            <div class="col-xs-12">
				<h1>Hello world!</h1>
				<Quote>
					<h3 slot="title">{{ quote.quoteTitle }}</h3>
					<h4 slot="subtitle">Quote nr 21</h4>
					<p slot="content"><q>{{ quote.quoteContent }}</q></p>
				</Quote>
            </div>
        </div>
    </div>
</template>

<script>
    import Quote from './components/Quote.vue'

    export default {
		components: {
			Quote
		},
		data: function() {
			return {
				quote: {
					quoteTitle: 'The Quote of the day:',
					quoteContent: 'To envision the future, one must learn from the past to create a new tomorrow.'
				}
			}
		}
    }
</script>

<style scoped>
h1 {
	padding: 30px;
}
div {
	margin: 0 auto;
	text-align: center;
}
h3 {
	color:rgb(112, 162, 180)
}
</style>
