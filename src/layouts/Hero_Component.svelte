<div class="hero_component">
	<Grid stack>
		<Col col="7">
			<div class="hero_content">
				<Hero>
					<h1>Metis is your new</h1>
					<h1 class="text-primary">virtual materials lab</h1>
					<Button variant="secondary" size="xl">Download now</Button>
				</Hero>
			</div>
		</Col>
		<Col col="5">
			<img src="assets/img/hero.jpg" alt="img" />
		</Col>
	</Grid>
</div>

<script lang="ts" context="module">
	import { Hero, Button, Grid, Col } from 'svelte-spectre';
</script>

<style lang="scss">
	.hero_component {
		width: 100%;
		height: calc(100vh - 145px);
		display: flex;
		align-items: center;
		margin: 0px;
		padding-left: 50px;
		padding-right: 0px;
		@media (max-width: 1024px) {
			height: calc(70vh - 145px);
		}
	}
	.hero_component .hero_content {
		display: flex;
		height: 100%;
		align-items: center;
		@media (max-width: 1024px) {
			margin-top: 48px;
		}
	}
	.hero_component h1 {
		font-size: 112px;
		margin-bottom: 0px;
		@media (max-width: 1844px) {
			font-size: 64px;
		}
		@media (max-width: 1024px) {
			font-size: 48px;
		}
		@media (max-width: 837px) {
			font-size: 38px;
		}
	}
	.hero_component h1.text-primary {
		margin-bottom: 48px;
	}
	.hero_component img {
		width: 100%;
		height: calc(100vh - 145px);
		margin-bottom: 0px;
		@media (max-width: 1024px) {
			height: calc(70vh - 145px);
		}
	}
</style>
