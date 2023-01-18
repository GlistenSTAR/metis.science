<Spectre>
	<Header />
	<Main />
	<!-- <Footer /> -->
</Spectre>

<script lang="ts" context="module">
	import { Spectre } from 'svelte-spectre';
	import { Header, Footer } from './views/';
	import { Main } from './layouts/';
	import { darkTheme } from '@/stores/theme';
</script>

<style>
	@import '@slidy/svelte/dist/slidy.css';
	@import './assets/global.css';
</style>
