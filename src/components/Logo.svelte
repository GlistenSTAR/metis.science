<span {id} style:--width={size}>
	<Icon size="4x" {color}>
		{@html MetisLogo}
	</Icon>
</span>

<script lang="ts" context="module">
	import { Icon } from 'svelte-spectre';
	import MetisLogo from '@/assets/img/metis.svg';
</script>

<script lang="ts">
	export let id = 'metis';
	export let size = '7em';
	export let color: any = 'dark';
</script>

<style lang="scss">
	span {
		width: var(--width);
		height: 100%;
	}
	@media (prefers-color-scheme: dark) {
		:global(#metis) {
			color: $gray-color;
		}
	}
	@media (prefers-color-scheme: light) {
		:global(#metis) {
			color: $dark-color;
		}
	}
	:global([color-scheme='dark']) {
		:global(#metis) {
			color: $gray-color;
		}
	}
	:global([color-scheme='light']) {
		:global(#metis) {
			color: $dark-color;
		}
	}
</style>
