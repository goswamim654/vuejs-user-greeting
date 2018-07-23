<template>
	<input :value="getMessage" @keyup="handleMessageInputChanges($event)">
</template>
<script>
	import { mapGetters, mapActions } from 'vuex'
	import { CHANGE_MESSAGE, INCREMENT_COUNTER } from '../vuex/mutation_types'


	export default {
		computed: mapGetters(['getMessage']),
		methods: mapActions(['handleMessageInputChanges'])
	}
</script>