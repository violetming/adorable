  <template>
	<view>
		<view class="status_bar">
		<!-- 这里是状态栏 -->
		</view>	
		<!-- F1 -->
		<view class="f1box1">
			<view class="f1box2">
				<image src="../../static/img/walkTheDog.svg" mode=""></image>
				<text>遛狗</text>
			</view>
			<view class="f1box2">
				<image src="../../static/img/walkTheDog.svg" mode=""></image>
				<text>遛狗</text>
			</view>
			<view class="f1box2">
				<image src="../../static/img/walkTheDog.svg" mode=""></image>
				<text>遛狗</text>
			</view>
			<view class="f1box2">
				<image src="../../static/img/walkTheDog.svg" mode=""></image>
				<text>遛狗</text>
			</view>
			<view class="f1box2">
				<image src="../../static/img/walkTheDog.svg" mode=""></image>
				<text>遛狗</text>
			</view>
		</view>
		<!-- F2 -->
		<view class="f2box1">
			<button>快速发布</button>
		</view>
		<!-- F3 -->
		<view class="f3box1">
			<view class="f3box2">
				<view class="f3box3top">
					<view class="f3box3topleft">
						<text>每天楼下遛狗</text>
						<text>胜利桥东府东公馆1单元</text>
					</view>
					<text style="color: #f4ae3e;font-weight: bold;">50元/小时</text>
				</view>
				<button>应聘</button>
			</view>
			<view class="f3box2">
				<view class="f3box3top">
					<view class="f3box3topleft">
						<text>每天楼下遛狗</text>
						<text>胜利桥东府东公馆1单元</text>
					</view>
					<text style="color: #f4ae3e;font-weight: bold;">50元/小时</text>
				</view>
				<button>应聘</button>
			</view>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
			}
		},
		methods: {
			
		}
	}
</script>

<style lang="scss">
  .status_bar {
      height: var(--status-bar-height);
      width: 100%;
			background-color: #f4ae3e;
  }
	// F1
	.f1box1{
		width: 90%;
		margin: 40rpx auto;
		display: flex;
		justify-content: space-around;
		.f1box2{
			display: flex;
			flex-direction: column;
			width: 115rpx;
			
			image{
				width: 100rpx;
				height: 100rpx;
			}
			text{
				text-align: center;
			}
		}
	}
	// F2
	.f2box1{
		width: 90%;
		margin: 40rpx auto;
		button{
			background-color: #f4ae3e;
			color: #ffffff;
			&:active{
				opacity: 0.5;
			}
		}
	}
// F3
.f3box1{
	.f3box2{
		width: 90%;
		margin: 50rpx auto;
		display: flex;
		padding: 10rpx;
		background-color: #ffffff;
		border-radius: 10rpx;
		align-items: center;
		justify-content: space-between;
		.f3box3top{
			display: flex;
			justify-content: space-between;
			border-bottom: 1px solid #d6d6d6;
			margin-bottom: 10rpx;
			.f3box3topleft{
				display: flex;
				flex-direction: column;
				text{
					margin: 15rpx 8rpx;
				}
			}
		}
		button{
			width: 130rpx;
			height: 130rpx;
			background-color: #f4ae3e;
			color: #ffffff;
			line-height: 130rpx;
			margin: 0;
		}
	}
}
</style>
