<template>
	<view>
		<view class="f3box">
			<view class="f3box1">
			<uni-search-bar 
			bgColor="#eeeeee"
			class="uni-mt-10" 
			radius="100" 
			placeholder="关键字搜索" 
			clearButton="none" 
			cancelButton="none"/>
			</view>
			<view v-for="item in 10" class="f3box2">
				<view class="f3box2top">
					<image src="../../static/img/slideshow2.jpg" mode=""></image>
					<view class="f3box2right">
						<text>喵呜阿旺宠物医院(24小时)</text>
						<text>♥♥♥♥♥♥</text>
						<text class="f3box2botton">胜利桥东</text>
					</view>
				</view>
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
	.f3box{
		.f3box1{
			.uni-mt-10{
				width:90%;
				margin: 0 auto;
			}
		}
		.f3box2{
			width: 90%;
			margin: 10rpx auto;
			background-color: #f4ae3e;
			padding: 10rpx;
			border-radius: 10rpx;
			.f3box2top{
				display: flex;
				image{
					width: 230rpx;
					height: 175rpx;
					border-radius: 10rpx;
				}
				.f3box2right{
					
					display: flex;
					flex-direction: column;
					justify-content: flex-end;
					margin: 0 20rpx;
					text{
						margin: 5rpx 0;
					}
					.f3box2botton{
						margin: auto 0;
					}
				}
			}
		}
	}
</style>
