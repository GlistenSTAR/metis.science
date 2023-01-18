<div class="goal">
	<Grid stack>
		<Col col="6">
			<h1>Metis provides the rich web-based graphical user interface (GUI) for</h1>
		</Col>
		<Col col="6">
			<ul class="mb-9">
				{#each menus as item, index}
					<!-- svelte-ignore a11y-click-events-have-key-events -->
					<li class="menu {active_tab == index && 'active'}" on:click={() => activeTab(index)}>
						<h1>{item.text}</h1>
						{#if active_tab == index}
							<!-- svelte-ignore a11y-img-redundant-alt -->
							<img src={item.img} alt="image" />
						{/if}
					</li>
				{/each}
			</ul>
			<h2 class="goal_bottom_text">The new simulation codes and parameter optimization methods can be easily added.</h2>
		</Col>
	</Grid>
</div>

<script lang="ts">
	import { Grid, Col } from 'svelte-spectre';

	const menus = [
		{ text: `cheap on-demand cloud simulations`, img: 'assets/img/cloud-runs.png' },
		{ text: `digesting the experiments data`, img: 'assets/img/all-data.png' },
		{ text: `analyzing and comparing the data`, img: 'assets/img/optimade-search.png' },
		{ text: `exporting and sharing the data across your lab`, img: 'assets/img/content-organizer.png' },
	];

	let active_tab = 0;

	const activeTab = (index) => {
		active_tab = index;
		console.log(active_tab);
	};
</script>

<style lang="scss">
	.goal {
		position: relative;
		background: #111;
		padding: 160px 0 160px 50px;
		color: white;
	}
	.goal h1 {
		font-size: 48px;
	}

	.goal .menu {
		display: flex;
		align-items: center;
		counter-increment: section;
		cursor: pointer;
	}
	.goal .menu.active h1 {
		background: #333;
	}
	.goal .menu h1 {
		border-bottom: 1px solid #adadad;
		padding: 36px 0;
		font-size: 36px;
		width: 100%;
	}
	.goal .menu:nth-child(1) h1 {
		border-top: 1px solid #adadad;
	}
	.goal .menu::before {
		content: '(' counter(section, lower-alpha) ') ';
		font-size: 28px;
		font-weight: 300;
		margin-right: 28px;
	}
	.goal img {
		position: absolute;
		left: 0;
		bottom: 0;
		width: 46%;
		height: 509px;
		z-index: 1;
		visibility: hidden;
		transition: all 0.3s ease-in-out;
		opacity: 0.9;
	}
	.goal_bottom_text {
		margin-left: 77px;
		font-size: 24px;
		width: 100%;
		font-weight: 300;
		width: 80%;
	}
	@media (max-width: 1580px) {
		.goal img {
			width: 45%;
			height: 409px;
		}
	}
</style>
