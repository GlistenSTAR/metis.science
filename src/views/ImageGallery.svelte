<section class="image-gallery">
	<Grid stack>
		{#each images as image, i}
			<Col col="4">
				<Button on:click={() => setIndex(i)}>
					<img width="150" height="150" src={image.src} alt={image.caption} title={image.caption} />
				</Button>
			</Col>
		{/each}
	</Grid>
</section>

<script lang="ts" context="module">
	import { Button, Col, Grid } from 'svelte-spectre';
</script>

<script lang="ts">
	export let images: { [key: string]: string | number }[] = [];
	export let index: number;
	export let open = false;
	function setIndex(i: number) {
		open = !open;
		index = i;
	}
</script>

<style lang="scss">
	.image-gallery {
		max-width: 500px;
		margin: auto;
		padding-top: 3rem;
		:global(button) {
			width: 100%;
			height: auto !important;
		}
		img {
			max-width: 100%;
			object-fit: contain;
			height: auto;
		}
	}
</style>