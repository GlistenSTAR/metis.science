<div class="backend">
	<Grid stack>
		<Col col="10">
			<div class="backend_title">scientific backend</div>
			<div class="backend_text">
				The scientific backend is written in Python and able to manage complex multi-level simulation workflows via the AiiDA workflow manager. It
				orchestrates scientific codes TOPAS, FullProf, VASP, Quantum Espresso, CRYSTAL, etc. in the clouds of well-known commodity providers.
			</div>
		</Col>
		<Col col="2">
			<img class="backend_code_img" src="assets/img/code.jpg" alt="code" />
		</Col>
	</Grid>
	<Grid stack>
		<Col col="6">
			<div class="backend_techs">
				<div class="backend_row">
					<img src="assets/img/backend/tech1.svg" alt="tech_stack" />
					<img src="assets/img/backend/tech2.svg" alt="tech_stack" />
				</div>
				<div class="backend_row">
					<img src="assets/img/backend/tech3.png" alt="tech_stack" />
					<img src="assets/img/backend/tech4.png" alt="tech_stack" />
				</div>
				<div class="backend_row">
					<img src="assets/img/backend/tech5.svg" alt="tech_stack" />
					<img src="assets/img/backend/tech6.png" alt="tech_stack" />
				</div>
			</div>
		</Col>
		<Col col="6">
			<div class="backend_bottom">
				<div class="backend_description">
					The scientific backend supports Microsoft Azure, Hetzner, Upcloud, and Google Cloud. All the scientific logic is encapsulated here. Download
					and deploy it at your own web-server.
				</div>
				<Button variant="primary" size="xl">Download now</Button>
			</div>
		</Col>
	</Grid>
</div>

<script lang="ts" context="module">
	import { Grid, Col, Button } from 'svelte-spectre';
</script>

<style lang="scss">
	.backend {
		padding: 160px 50px 200px;
		color: white;
		position: relative;
		background: #111;
		overflow: hidden;
	}
	.backend_title {
		position: absolute;
		top: 171px;
		left: 50px;
	}
	.backend_text {
		text-indent: 310px;
		width: 1386px;
		margin-bottom: 177px;
		font-size: 36px;
		line-height: 134%;
	}
	.backend_code_img {
		position: absolute;
		top: 160px;
		right: -300px;
		height: 354px;
		width: auto;
		object-fit: contain;
		z-index: 1;
	}

	.backend_techs {
		margin-right: 100px;
		margin-left: -50px;
	}
	.backend_row {
		display: flex;
		padding: 54px 0 54px 50px;
		justify-content: flex-end;
		border-bottom: 1px solid #adadad;
	}
	.backend_row img + img {
		margin-left: 72px;
	}
	.backend_row:nth-child(1) {
		border-top: 1px solid #adadad;
	}
	.backend_row:last-child {
		justify-content: flex-start;
	}

	.backend_bottom {
		display: flex;
		height: 100%;
		flex-direction: column;
		align-items: flex-start;
		justify-content: flex-end;
	}
	.backend_description {
		margin-bottom: 60px;
		font-size: 28px;
		line-height: 136%;
	}
</style>
