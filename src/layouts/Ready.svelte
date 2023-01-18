<div class="ready">
	<img src="assets/img/dots.png" alt="dots" class="dots" />
	<div class="ready_content">
		<Hero>
			<h1>Ready to get started?</h1>
			<h1 class="detail">Download your digital materials lab assistant right now.</h1>
			<Button variant="secondary" size="xl">Download now</Button>
		</Hero>
	</div>
	<img src="assets/img/dots.png" alt="dots" class="bottom_dots" />
</div>

<script lang="ts" context="module">
	import { Hero, Button } from 'svelte-spectre';
</script>

<style lang="scss">
	.ready {
		position: relative;
		margin-top: 100px;
		/* color: #353438; */
	}
	.ready img.dots {
		position: absolute;
		z-index: -1;
		top: -69px;
		left: 0;
		height: 169px;
		width: 351px;
	}
	.ready img.bottom_dots{
		position: absolute;
		z-index: -1;
		bottom: -69px;
		right: 0;
		height: 169px;
		width: 351px;
	}
	.ready_content {
		padding: 180px 0 152px;
		position: relative;
		display: flex;
		align-items: center;
		flex-direction: column;
		text-align: center;
	}
	.ready_content h1 {
		font-size: 112px;
		line-height: 108%;
		font-weight: 500;
	}
	.ready_content h1.detail {
		font-size: 36px;
		margin-bottom: 60px;
	}
</style>
