<template>
    <div class="container">
        <div class="row">
            <div class="col-xs-12">
				<h1>Workout Examples</h1>
				<button @click="selectedComponent = 'Strength'">Strength</button>
				<button @click="selectedComponent = 'Hypertrophy'">Hypertrophy</button>
				<button @click="selectedComponent = 'Endurance'">Endurance</button>
				<hr>
				<component :is="selectedComponent">
					<h3 slot="title">{{ title }}</h3>
					<!-- <p slot="author">{{author }}</p> -->
					<p slot="duration">{{duration }}</p>
				</component>
            </div>
        </div>
    </div>
</template>

<script>
    import Strength from './components/Strength.vue'
    import Hypertrophy from './components/Hypertrophy.vue'
    import Endurance from './components/Endurance.vue'

    export default {
		data: function() {
			return {
				title: 'Upper-body Strength',
				duration: '10 weeks',
				author: 'Rocky Balboa',
				
				selectedComponent: 'Strength'
			}
		},

		components: {
			Strength,
			Hypertrophy,
			Endurance
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

</style>
