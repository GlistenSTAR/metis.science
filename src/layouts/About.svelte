<div class="about">
	<span class="about_title">about the name</span>
	<div class="about_content">
		The <span class="highlight">Metis</span> name stands for the Greek mythological deity of <span class="highlight">wisdom</span> and
		<span class="highlight">deep thought.</span>
	</div>
	<div class="about_bottom">From the solid state physics foundations, Metis accumulates the materials knowledge and derives the materials wisdom.</div>
	<div class="about_plot">
		<img src="assets/img/Vector.png" alt="vector_image" />
	</div>
</div>

<style lang="scss">
	.about {
		background: #111;
		padding: 160px 50px 320px;
		position: relative;
		color: white;
		overflow: hidden;
		line-height: 1.1;
	}
	.about_title {
		position: absolute;
		top: 172px;
		left: 50px;
	}
	.about_content {
		width: 1110px;
		font-size: 68px;
		text-indent: 280px;
		@media (max-width: 1440px) {
			font-size: 52px;
		}
		@media (max-width: 1100px) {
			width: 80%;
			font-size: 42px;
			text-indent: 140px;
		}
	}
	.about_content .highlight {
		background: linear-gradient(
			104deg,
			rgba(87, 85, 217, 0) 20px,
			rgb(87, 85, 217) 20px,
			rgb(87, 85, 217) calc(100% - 20px),
			rgba(255, 255, 255, 0) calc(100% - 20px)
		);
		color: white;
		padding: 0 20px;
		line-height: 1.3;
	}
	.about_bottom {
		font-size: 28px;
		position: absolute;
		bottom: 160px;
		right: 149px;
		width: 645px;
		@media (max-width: 1100px) {
			font-size: 24px;
			right: 0px;
		}
	}
	.about_plot {
		width: 657px;
		height: 380px;
		position: absolute;
		bottom: 93px;
		right: -173px;
	}
</style>
