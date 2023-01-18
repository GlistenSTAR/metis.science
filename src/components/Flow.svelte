<div class="flow">
	<div class="flow_wrapper">
		<div class="flow_item">
			<span class="sign">#</span>
			<span>Digital materials lab assistant</span>
		</div>
		<div class="flow_item">
			<span class="sign">#</span>
			<span>Free open-source virtual materials environment</span>
		</div>
		<div class="flow_item">
			<span class="sign">#</span>
			<span>Highly-scalable cheap scientific simulations in the cloud</span>
		</div>
		<div class="flow_item">
			<span class="sign">#</span>
			<span>Modular reusable component-based system</span>
		</div>
	</div>
</div>

<style lang="scss">

	.flow {
		padding: 40px 0;
		background: #111;
		color: white;
		border-bottom: 1px solid #adadad;
		border-top: 1px solid #adadad;
		overflow: hidden;
		margin-top: -8px;
		display: flex;
	}
	.flow_wrapper{
		height: 100%;
		width: 200vw;
		display: flex;
		animation: running-anim 10s forwards infinite linear;
		@keyframes running-anim {
            from {
                transform: translateX(0)
			}
            to {
                transform: translateX(-39.5vw)
			}
		}
		@media (max-width: 1016px) {
			width: 300vw;
		}
	}
	
	.flow_item{
		display: flex;
		align-items: center;
		margin-right: 180px;
		width: max-content;
		@media (max-width: 1556px) {
			margin-right: 40px;
		}
	}
	.flow_item span{
		font-size: 28px;
		@media (max-width: 1276px) {
			font-size: 22px;
		}
	}
	.flow_item .sign{
		font-size: 40px;
		margin-right: 5px;
		@media (max-width: 1276px) {
			font-size: 24px;
		}
	}
</style>
