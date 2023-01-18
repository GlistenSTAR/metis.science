<div class="bff">
	<Grid stack>
		<Col col="6">
			<div class="bff_box">
				<div class="bff_title">backend-for-frontend</div>
				<div class="bff_content">
					The Metis backend-for-frontend (BFF) deals with the user-related logics (accounts, access, permissions, etc.). All the user and data
					management is encapsulated here. Download and deploy it at your own web-server.
				</div>
				<div class="bff_bottom_box">
					<div class="bff_bottom">
						<img src="assets/img/node.png" alt="node" />
						<Logo size="4em" />
					</div>
					<Button variant="secondary" size="xl">Download now</Button>
				</div>
			</div>
		</Col>
		<Col col="6">
			<!-- <img src="assets/img/code_bg.jpg" alt="code" /> -->
			<CodeEditor {code} lang="css" loc {...$$restProps} />
		</Col>
	</Grid>
</div>

<script lang="ts">
	import { Grid, Col, Button } from 'svelte-spectre';
	import { Logo } from '@/components/index';
	import CodeEditor from 'svelte-code-editor';

	let code = `				line-height: 1;
				font-size: 9px;
				color: black;
				padding-top: 8px;
			}
		}
		li.triangle_col {
			font-size: 22px;
			border: none;
			display: flex;
			align-items: flex-end;
			justify-content: center;`;
</script>

<style lang="scss">
	.bff {
		padding: 146px 50px 220px;
	}
	.bff_box {
		position: relative;
	}
	.bff_title {
		position: absolute;
		top: 11px;
		left: 0;
		font-weight: 300;
		font-size: 20px;
		line-height: 24px;
	}
	.bff_content {
		text-indent: 308px;
		margin-bottom: 80px;
		font-size: 36px;
		line-height: 134%;
	}
	.bff_bottom_box {
		display: flex;
		align-items: flex-end;
	}
	.bff_bottom {
		padding: 30px 0;
		display: flex;
		align-items: center;
		width: 461px;
		border-top: 1px solid #cdcdcd;
		border-bottom: 1px solid #cdcdcd;
		margin-right: 154px;
	}
	.bff_bottom img {
		width: auto;
		object-fit: contain;
		height: 40px;
		margin-right: 70px;
	}
</style>
