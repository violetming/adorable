<template>
	<view>
		<view class="status_bar">
							<!-- 这里是状态栏 -->
						</view>	
						<!-- F1 -->
			<view class="title">
				<text class="txtq">
					同城
				</text>
			<uni-search-bar class="uni-mt-10" radius="100" placeholder="关键字搜索" clearButton="none" cancelButton="none"/>
		</view>
		<!-- F2 -->
		<view class="f2title">
			<view class="f2box">
			<view class="f2box1">
				<image src="../../static/img/part-time.svg" mode=""></image>
			</view>
				<text>兼职</text>
			</view>
			<view class="f2box">
			<view class="f2box1">
				<image src="../../static/img/part-time.svg" mode=""></image>
			</view>
				<text>兼职</text>
			</view>
			<view class="f2box">
			<view class="f2box1">
				<image src="../../static/img/part-time.svg" mode=""></image>
			</view>
				<text>兼职</text>
			</view>
			<view class="f2box">
			<view class="f2box1">
				<image src="../../static/img/part-time.svg" mode=""></image>
			</view>
				<text>兼职</text>
			</view>
		</view>
		<!-- F3 -->
		<view class="f3box">
			<view class="f3box1">
				<uni-icons type="email-filled" size="30"></uni-icons>
				<text>附近</text>
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
	.title{
		display: flex;
		align-items: center;
		width: 750rpx;
		background-color:#f4ae3e ;
		justify-content: flex-start;
		height: 90rpx;
		.txtq{
			display: flex;
			font-size: 15px;
			font-weight: bold;
			margin-left: 20rpx;
			color: #ffffff;
			margin:0 40rpx;
		}
		.uni-mt-10{
			width: 530rpx;
		}
		.search{
			display: block;
			background-color: #ffffff;
			border-radius: 30rpx;
			width: 500rpx;
			margin: 0 30rpx;
			height: 60rpx;
		}
	}
	// F2
	.f2title{
		display: flex;
		justify-content: space-evenly;
		text-align: center;
		.f2box{
			margin-top: 30rpx;
			text{
				display: inline-block;
				margin-top: 15rpx;
			}
			.f2box1{
			display: flex;
			flex-direction: column;
			width: 140rpx;
			height: 140rpx;
			justify-content: center;
			align-items: center;
			background-color: #f4ae3e;
			border-radius: 10rpx;
			image{
				width: 100rpx;
				height: 100rpx;
			}
			}
		}
	}
</style>
