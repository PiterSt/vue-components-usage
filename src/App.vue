<template>
    <div class="container">
        <div class="row">
            <div class="col-xs-12">
				<h1>Hello world!</h1>
				<button @click="selectedComponent = 'Quote'">Quote</button>
				<button @click="selectedComponent = 'Author'">Author</button>
				<button @click="selectedComponent = 'NewQuote'">NewQuote</button>
				<p>{{ selectedComponent }}</p>
				<hr>
				<component :is="selectedComponent">
					<h3 slot="title">{{ quote.quoteTitle }}</h3>
					<p slot="subtitle">Quote nr 21</p>
					<p slot="content"><q>{{ quote.quoteContent }}</q></p>
				</component>
				<!-- <Quote>
					
				</Quote> -->
            </div>
        </div>
    </div>
</template>

<script>
    import Quote from './components/Quote.vue'
    import Author from './components/Author.vue'
    import NewQuote from './components/NewQuote.vue'

    export default {
		components: {
			Quote,
			Author,
			NewQuote
		},
		data: function() {
			return {
				quote: {
					quoteTitle: 'The Quote of the day:',
					quoteContent: 'To envision the future, one must learn from the past to create a new tomorrow.'
				},
				selectedComponent: 'Quote'
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
