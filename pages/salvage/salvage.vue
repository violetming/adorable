<template>
	<view>
		<!-- F1 -->
		<view v-for="item in 5" class="f1box1">
			<view class="f1box2">
				<image src="../../static/img/yisheng.png" mode="scaleToFill"></image>
				<view class="f1box3">
					<view class="f1box4">
						<text>姓名</text>
						<text>发布时间</text>
					</view>
					<text class="f1box31">寻狗启示，迎泽大街附近走丢，边牧，脖子上有项圈！他叫汪汪！</text>
				</view>
			</view>
				<view class="f1box5">
					<image src="../../static/img/adopt2.jpg" mode="scaleToFill"></image>
					<image src="../../static/img/adopt2.jpg" mode="scaleToFill"></image>
					<image src="../../static/img/adopt2.jpg" mode="scaleToFill"></image>
				</view>
		</view>
		<!-- F2 -->
		<view class="f2box1">
			<button>快速发布</button>
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
	// F1
.f1box1{
	width: 90%;
	margin: 0 auto;
	padding-bottom: 20rpx;
	margin-bottom: 10rpx;
	border-bottom: 1px solid #d6d6d6;
	.f1box2{
		margin-top: 30rpx;
		margin-bottom: 10rpx;
		display: flex;
		>image{
			display: block;
			width: 150rpx;
			height: 110rpx;
			border-radius: 50%;
		}
		.f1box3{
			.f1box4{
				margin: 8rpx 20rpx;
				display: flex;
				justify-content: space-between;
			}
			.f1box31{
				display: inline-block;
				margin:0 20rpx;
			}
		}
	}
		.f1box5{
			display: flex;
			justify-content: space-around;
			>image{
				width: 200rpx;
				height: 200rpx;
				border-radius: 10rpx;
				
			}
		}
}
// F2
	.f2box1{
		position:fixed;
		bottom: 0;
		width: 100%;
        display: flex; // 添加弹性布局
        justify-content: center; // 水平居中
        align-items: center; // 垂直居中
		button{
			width: 90%;
			background-color: #f4ae3e;
			color: #ffffff;
			&:active{
				opacity: 0.5;
			}
		}
	}
</style>
