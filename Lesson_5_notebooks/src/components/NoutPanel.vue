<template>
	<card-nout v-for="nout in noutListData" :nout-data="nout" :key="nout.id" />

 
</template>

<script>
import CardNout from './CardNout.vue'
	export default {
		name:'NoutPanel',
		components:{
			CardNout
		},
		props: {
		noutListData: {
				type: Array,
				default:()=>[], 
			},
		},
	}
</script>

<style lang="scss" scoped>

</style>