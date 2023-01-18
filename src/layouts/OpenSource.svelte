<div class="open_source">
	<img src="assets/img/dots.png" alt="dots" />
	<Grid stack>
		<Col col="9">
			<span class="highlight">Metis is free and fully open source.</span>
			<h1 class="text-black">We advocate this code for our partner organizations, synchrotrons, XRPD, and materials science community in general.</h1>
		</Col>
		<div class="p-centered">
			<Col col="3">
				<Button variant="secondary" size="xl">Download now</Button>
			</Col>
		</div>
	</Grid>
</div>

<script lang="ts" context="module">
	import { Grid, Col, Button } from 'svelte-spectre';
</script>

<style lang="scss">
	.open_source {
		position: relative;
		padding: 220px 66px;
		font-weight: 500;
	}
	.open_source img {
		position: absolute;
		z-index: -1;
		top: -69px;
		left: 0;
		height: 169px;
		width: 351px;
	}
	.open_source span,
	.open_source h1 {
		font-size: 68px;
	}
    .open_source span{
        line-height: 108%;
    }
    .open_source h1 {
        margin-bottom: 0px;
    }
	.open_source span.highlight {
		clip-path: polygon(20px 25%, 100% 25%, calc(100% - 20px) 100%, 0 100%) !important;
		background: linear-gradient(
			104deg,
			rgba(87, 85, 217, 0) 20px,
			rgb(87, 85, 217) 20px,
			rgb(87, 85, 217) calc(100% - 20px),
			rgba(255, 255, 255, 0) calc(100% - 20px)
		);
		color: white;
		padding: 0 20px;
		padding-top: 10px;
		margin-left: -20px;
	}
</style>
