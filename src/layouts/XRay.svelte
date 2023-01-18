<div class="xray">
	<Grid stack>
		<Col col="6">
			<div class="xray_box mb-6">
				<div class="title">x-ray powder diffraction (XRPD)</div>
				<div class="content">
					Metis
					<span class="highlight1">supports scientific</span>
					<span class="highlight2">codes</span> TOPAS and FullProf for phase identification and Rietveld analysis.
				</div>
			</div>
			<img src="assets/img/xray.jpg" alt="xray" class="xray_img" />
		</Col>
		<Col col="6">
			<div class="xray_detail">
				<div class="content">All crystallographic formats and raw diffractometer data formats are recognized.</div>
				<div class="xray_detail_row">
					<div class="xray_item">
						<span class="sign">#</span>
						<span class="techs">TOPAS</span>
					</div>
					<div class="xray_item">
						<span class="sign">#</span>
						<span class="techs">FullProf</span>
					</div>
					<div class="xray_item">
						<span class="sign">#</span>
						<span class="techs">VASP</span>
					</div>
				</div>
				<div class="xray_detail_row">
					<div class="xray_item">
						<span class="sign">#</span>
						<span class="techs">Quantum Espresso</span>
					</div>
					<div class="xray_item">
						<span class="sign">#</span>
						<span class="techs">CRYSTAL</span>
					</div>
				</div>
				<div class="title">ab initio (first-principles) modeling</div>
				<div class="content">
					Metis supports scientific codes VASP, Quantum Espresso, and CRYSTAL to model the electronic structure of materials and to predict a wide
					range of physical properties, based on the only crystalline structure provided.
				</div>
			</div>
		</Col>
	</Grid>
</div>

<script lang="ts" context="module">
	import { Grid, Col } from 'svelte-spectre';
</script>

<style lang="scss">
	.xray_box {
		padding: 160px 50px 0;
		position: relative;
	}
	.xray_box .title {
		margin-bottom: 20px;
		font-size: 20px;
		line-height: 24px;
		font-weight: 300;
	}
	.xray_box .content {
		font-size: 68px;
		line-height: 108%;
		font-weight: 500;
	}
	.xray_box span.highlight1 {
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
		padding-top: 20px;
	}
	.xray_box span.highlight2 {
		clip-path: polygon(20px 25%, 100% 25%, calc(100% - 20px) 100%, 0 100%) !important;
		background: linear-gradient(
			104deg,
			rgba(87, 85, 217, 0) 20px,
			rgb(87, 85, 217) 20px,
			rgb(87, 85, 217) calc(100% - 20px),
			rgba(255, 255, 255, 0) calc(100% - 20px)
		);
		color: white;
		padding: 0 16px;
		padding-top: 5px;
	}
	.xray .xray_img {
		position: absolute;
		width: 42%;
		height: 862px;
	}

	.xray_detail {
		padding: 160px 0 0 30px;
	}
	.xray_detail .content {
		margin-bottom: 108px;
		font-size: 36px;
		line-height: 134%;
	}
	.xray_detail .xray_detail_row:nth-child(2) {
		border-top: 1px solid #cdcdcd;
	}
	.xray_detail .xray_detail_row {
		display: flex;
		font-size: 28px;
		line-height: 136%;
		border-bottom: 1px solid #cdcdcd;
		padding: 48px 0;
		width: 100%;
	}
	.xray_detail .xray_item {
		display: flex;
	}
	.xray_detail .xray_detail_row span.sign {
		font-size: 56px;
		font-weight: 500;
		margin-right: 20px;
	}
	.xray_detail .xray_detail_row span {
		margin-right: 40px;
	}
	.xray_detail .title {
		margin-bottom: 20px;
		font-size: 20px;
		line-height: 24px;
		font-weight: 300;
		margin-top: 108px;
	}
	.xray_detail .content {
		font-size: 48px;
		line-height: 116%;
		font-weight: 500;
	}

	@media (max-width: 1650px) {
		.xray .xray_img {
			width: 45%;
		}
	}
</style>
