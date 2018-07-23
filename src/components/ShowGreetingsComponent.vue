<template>
	<div>
		<h1>{{ getMessage }}</h1>
		<div>The message has been changed {{ getCounter }} times</div><br>
	</div>
</template>
<script>
	import { mapGetters } from 'vuex'
	export default {
		computed: mapGetters(['getMessage', 'getCounter'])
	}
</script>