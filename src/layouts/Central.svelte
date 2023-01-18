<div class="central">
	<div class="central_dots">
		<img src="assets/img/dots.png" alt="dots" />
	</div>
	<div class="central_inner">
		<div class="central_title">Metis is the browser-based online collaborative system for the materials data management.</div>
		<div class="central_text">The X-ray powder diffraction (XRPD) data, phase identification, and ab initio (first-principles) modeling is supported.</div>
		<Logo />
	</div>
</div>

<script lang="ts" context="module">
	import { Logo } from '@/components';
</script>

<style lang="scss">
	.central {
		position: relative;
		padding: 180px 0;
		text-align: center;
	}
	.central .central_dots {
		position: absolute;
		z-index: -1;
		top: -69px;
		left: 0;
		height: 169px;
		width: 351px;
	}
	.central .central_inner {
		width: 100%;
		margin: 0 auto;
		display: flex;
		align-items: center;
		flex-direction: column;
		line-height: 1.1;
		padding-left: 120px;
		padding-right: 120px;
	}
	.central .central_title {
		margin-bottom: 40px;
		font-size: 68px;
	}
	.central .central_text {
		width: 1058px;
		margin-bottom: 60px;
		font-size: 36px;
	}
	@media (max-width: 1020px) {
		.central .central_inner {
			padding-left: 40px;
			padding-right: 40px;
		}
	}
</style>
