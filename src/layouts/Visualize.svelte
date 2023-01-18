<div class="visualize">
	<Grid stack>
		<Col col="5">
			<img src="assets/img/frost.jpg" alt="frost" />
		</Col>
		<Col col="7">
			<div class="visualize_text">
				<div class="visualize_box">
					<div class="title">online GUI app</div>
					<div class="context">
						The Metis GUI visualizes crystal structures and X-ray patterns as you expect it. It is built on a modular components user interface kit.
						All the human interactions are encapsulated here. Download and deploy it at your own web-server.
					</div>
				</div>
				<div class="visualize_bottom_box">
					<div class="visualize_bottom">
						<img src="assets/img/svelte.svg" alt="svelte" />
						<Logo size="4em" />
					</div>
					<Button variant="secondary" size="xl">Download now</Button>
				</div>
			</div>
		</Col>
	</Grid>
	<img src="assets/img/dots.png" alt="dots" class="dots" />
</div>

<script lang="ts" context="module">
	import { Grid, Col, Button } from 'svelte-spectre';
	import { Logo } from '@/components/index';
</script>

<style lang="scss">
	.visualize {
		position: relative;
	}
	.visualize img {
		width: 100%;
		height: 685px;
		object-fit: cover;
	}
	.visualize_text {
		position: relative;
		height: 100%;
		display: flex;
		flex-direction: column;
		justify-content: flex-end;
		padding-left: 120px;
		padding-right: 80px;
	}
	.visualize_box {
		position: relative;
	}
	.visualize_text .title {
		position: absolute;
		top: 11px;
		left: 0;
		font-size: 20px;
		line-height: 24px;
		font-weight: 300;
	}
	.visualize_text .context {
		text-indent: 308px;
		margin-bottom: 80px;
		font-size: 36px;
		line-height: 134%;
	}

	.visualize_bottom_box {
		display: flex;
		align-items: flex-end;
	}
	.visualize_bottom {
		padding: 30px 0;
		display: flex;
		align-items: center;
		width: 461px;
		border-top: 1px solid #cdcdcd;
		border-bottom: 1px solid #cdcdcd;
		margin-right: 154px;
	}
	.visualize_bottom img {
		width: auto;
		object-fit: contain;
		height: 40px;
		margin-right: 70px;
	}

	img.dots {
		position: absolute;
		z-index: -1;
		bottom: -69px;
		left: 0;
		height: 169px;
		width: 351px;
	}
</style>
