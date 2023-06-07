<template>
	<view>
				<view class="status_bar">
					<!-- 这里是状态栏 -->
				</view>	
				<!-- F1 -->
			<view class="title">
				<text class="txtq">
					发现
				</text>
<uni-search-bar class="uni-mt-10" radius="100" placeholder="关键字搜索" clearButton="none" cancelButton="none"/>
				<uni-icons style="color: #ffffff;" type="email-filled" size="30"></uni-icons>
			</view>
<!-- F2轮播 -->
			<view>
				<swiper class="swiper" circular  autoplay="autoplay" interval="5000"
					:duration="500">
					<swiper-item>
						<view class="swiper-item uni-bg-red">
							<image class="width:100%" src="../../static/img/slideshow1.jpg" mode="scaleToFill"></image>
						</view>
					</swiper-item>
					<swiper-item>
						<view class="swiper-item uni-bg-green">
							<image src="../../static/img/slideshow2.jpg" mode="scaleToFill"></image>
						</view>
					</swiper-item>
					<swiper-item>
						<view class="swiper-item uni-bg-blue">
							<image src="../../static/img/slideshow3.jpg" mode="scaleToFill"></image>
						</view>
					</swiper-item>
				</swiper>
			</view>
			<!-- F3宠物领养 -->
			<view >
				<view class="F3title">
					<view>
						<view class="F3titleTop">
								<view class="F3left">
									<uni-icons type="email-filled" size="30"></uni-icons>
									<text>宠物领养</text>
								</view>
							<text @click="jump('/pages/adoption/adoption')">更多..</text>
						</view>
						<view class="subject">
							<view class="subject1">
								<image src="../../static/img/adopt1.jpg" mode="scaleToFill"></image>
								<view class="textsubject">
									<text>来福</text>
									<text>金毛</text>
									<text>1岁6个月</text>
								</view>
							</view>
							<view class="subject1">
								<image src="../../static/img/adopt1.jpg" mode="scaleToFill"></image>
								<view class="textsubject">
									<text>来福</text>
									<text>金毛</text>
									<text>1岁6个月</text>
								</view>
							</view>
						</view>
					</view>
				</view>
			</view>
			<!-- F4 -->
			<view>
				<view class="f4title">
					<view class="f4titleTop">
							<view class="f4left">
								<uni-icons type="email-filled" size="30"></uni-icons>
								<text>问医生</text>
							</view>
						<text @click="jump('/pages/doctorlist/doctorlist')">更多..</text>
					</view>
					<view class="f4subject">
						<view class="f4subject1">
							<image src="../../static/img/yisheng.png" mode="scaleToFill"></image>
							<text>张三</text>
							<text>猫病从业3年</text>
						</view>
						<view class="f4subject1">
							<image src="../../static/img/yisheng.png" mode="scaleToFill"></image>
							<text>张三</text>
							<text>猫病从业3年</text>
						</view>
						<view class="f4subject1">
							<image src="../../static/img/yisheng.png" mode="scaleToFill"></image>
							<text>张三</text>
							<text>猫病从业3年</text>
						</view>
					</view>
				</view>
			</view>
			<!-- F5 -->
			<view class="F5title1">
				<text>常见问题</text>
				<view class="f5title">
					<view class="f5left">
						<text>猫瘟</text>
						<text>猫鼻支</text>
						<text>眼屎</text>
						<text>吐黄水</text>
						<text>不吃不喝</text>
					</view>
					<view class="f5right">
						<uni-icons style="color: #ffffff;"size="40" type="personadd-filled"></uni-icons>
						<text class="f5btn">在线问答</text>
					</view>
				</view>
			</view>
			<!-- F6 -->
			<view>
				<view class="f6titletop">
					<uni-icons type="email-filled" size="30"></uni-icons>
					<text>推荐文章</text>
				</view>
				<view v-for="item in 5" class="f6title">
					<view class="f6left">
						<text>狗狗的10中常见解析</text>
						<text>狗狗的尾巴代表什么？</text>
					</view>
					<image src="../../static/img/adopt2.jpg" mode="scaleToFill"></image>
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
			jump(url){
				uni.navigateTo({url})
			}
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
		justify-content: space-around;
		height: 90rpx;
		.txtq{
			display: flex;
			font-size: 15px;
			font-weight: bold;
			margin-left: 20rpx;
			color: #ffffff;
		}
		.uni-mt-10{
			width: 500rpx;
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
	.swiper{
		.swiper-item{
			width: 750rpx;
			image{
				display: block;
				width: 100%;
			}
		}
	}
	// F3
	.F3title{
		margin-top: 30rpx;
		width: 100%;
		flex-direction: column;
		display: flex;
		.F3titleTop{
			display: flex;
			justify-content: space-between;
			margin: 0 25rpx;
			.F3left{
				display: flex;
				align-items: center;
			}
		}
		.subject{
			display: flex;
			width: 750rpx;
			height: 150rpx;
			justify-content: space-around;
			image{
				display: block;
				width:200rpx;
				height: 150rpx;
				border-radius:10rpx ;
			}
			.subject1{
				padding: 10rpx;
				height: 150rpx;
				width: 330rpx;
				display: flex;
				box-shadow: 0 0 3px 1px #6d6d6d;
				background-color: #ffffff;
				border-radius: 10rpx;
				overflow: hidden;
				.textsubject{
					display: flex;
					flex-direction: column;
					justify-content: space-between;
					font-size: 13px;
					margin-left: 10rpx;
				}
			}
		}
	}
	// F4
.f4title{
	margin-top: 50rpx;
	.f4titleTop{
		display: flex;
		align-items: center;
		justify-content: space-between;
		margin: 0 20rpx;
		.f4left{
			display: flex;
			align-items: center;
		}
	}
	.f4subject{
	display: flex;
	justify-content: space-around;
		.f4subject1{
			display: flex;
			flex-direction: column;
			align-items: center;
			padding: 22rpx;
			background-color: #ffffff;
			width: 180rpx;
			height: 250rpx;
			image{
				display: block;
				width: 150rpx;
				height: 160rpx;
			}
			text{
			margin-top: 10rpx;
			font-size: 14px;
			}
		}
	}
}
// F5
.F5title1{
	margin: 30rpx 15rpx 0 15rpx;
	background-color: #ffffff;
	padding: 15rpx 10rpx;
.f5title{
	display: flex;
	align-items: center;
	background-color: #ffffff;
	    justify-content: space-around;
	.f5left{
		width:60%;
		text{
			display: inline-block;
			background-color: #f5dca6;
			padding: 7rpx  12rpx;
			margin:10rpx 15rpx 0 0;
			border-radius: 20px;
			font-size: 16px;
			color: #000000;
		}
	}
	.f5right{
		display: flex;
		width:29%;
		background-color: #f4ae3e;
		padding: 10rpx 5rpx;
		justify-content: center;
		align-items: center;
		border-radius: 10rpx;
		&:active{
			opacity: 0.6;
		}
	}
}
}
// F6
.f6titletop{
	display: flex;
	align-items: center;
	margin-top: 30rpx;
}
.f6title{
	display: flex;
	margin: 15rpx 30rpx;

	background-color: #ffffff;
	border-radius: 10rpx;
	    justify-content: space-around;
	.f6left{
		display: flex;
		flex-direction: column;
		width: 50%;
		justify-content: space-around;
	}
	image{
		display: block;
		width:200rpx;
		height: 150rpx;
		border-radius: 10rpx;
	}
}
	
</style>