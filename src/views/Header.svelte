<header class="p-1">
	<Navbar>
		<div slot="left" class="brand">
			<Logo size="5em" />
			<span>Metis</span>
		</div>
		<div slot="right" class="menu" on:click={ToggleMenu}>
			<div class="menu_item">
				{#if !is_open}
					<div class="burger" />
				{:else}
					<div class="cross" />
				{/if}
				<span>Menu</span>
			</div>
			{#if is_open}
				<div class="opened_menu">
					<li>Intro</li>
					<li>Why Metis?</li>
					<li>Technical Details</li>
					<li>Download and try</li>
					<li>GitHub</li>
				</div>
			{/if}
		</div>
	</Navbar>
</header>

<script lang="ts" context="module">
	import { Navbar, Icon } from 'svelte-spectre';
	import { Logo } from '@/components/index';
</script>

<script lang="ts">
	let is_open = false;

	const ToggleMenu = () => {
		is_open = !is_open;
	};
</script>

<style lang="scss">
	header {
		position: absolute !important;
		width: 100%;
	}
	.brand {
		display: flex;
		align-items: center;
		margin-top: 36px;
		margin-left: 50px;
		h1 {
			margin-bottom: 0px;
		}
	}
	span {
		font-size: 48px;
		@media (max-width: 1024px) {
			font-size: 28px;
		}
	}
	.menu {
		margin-right: 40px;
		margin-top: 36px;
		z-index: 9999;
		cursor: pointer;
		color: white;
	}
	.menu_item {
		display: flex;
		align-items: center;
	}
	.burger,
	.cross {
		width: 48px;
		height: 18px;
		margin-right: 18px;
		display: flex;
		flex-direction: column;
		justify-content: space-between;
		cursor: pointer;
	}

	.burger:after,
	.burger:before,
	.cross::after,
	.cross::before {
		content: '';
		background: white;
		display: block;
		width: 100%;
		height: 3px;
		transition: transform 0.3s ease-in-out;
	}
	.cross::before {
		transform: translateY(8px) rotate(-148deg);
	}
	.cross::after {
		transform: translateY(-8px) rotate(148deg);
	}

	.opened_menu {
		position: absolute;
		width: 320px;
		right: 40px;
		margin-top: 30px;
		padding: 10px;
		li {
			list-style: none;
			margin-bottom: 28px;
			font-size: 36px;
			text-align: right;
			color: #fff;
			@media (max-width: 1024px) {
				font-size: 28px;
			}
			@media (max-width: 724px) {
				font-size: 24px;
				margin-bottom: 18px;
			}
		}
	}
</style>
