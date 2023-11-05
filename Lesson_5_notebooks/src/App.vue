<template>
<nout-panel :nout-list-data="notebooksList" />
</template>

<script>
import NoutPanel from './components/NoutPanel.vue';
import {notebooksList} from './constants/3_data_notebooks';
export default {
  name: 'App',
  components: {
    NoutPanel
    
  },
	data() {
		return {
			notebooksList
		}
	},
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
