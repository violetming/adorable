<template>
	<!-- F1 -->
	<view>
		<view class="f1box1">
			<view class="f1box2">
				<uni-data-select
					v-model="value"
					:localdata="range"
					@change="change"
				></uni-data-select>
			</view>
			<view class="f1box3">
				<uni-data-select
					v-model="value"
					:localdata="range"
					@change="change"
				></uni-data-select>
			</view>
			<view class="f1box4">
				<uni-data-select
					v-model="value"
					:localdata="range"
					@change="change"
				></uni-data-select>
			</view>
		</view>
	<!-- F2 -->
	<view class="f2box1">
			<view class="f2box2">
				<image src="../../static/img/adopt1.jpg" mode="aspectFill"></image>
				<text>这里是狗狗的描述这里是狗狗的描述这里是狗狗的描述</text>
			</view>
			<view class="f2box2">
				<image src="../../static/img/adopt1.jpg" mode="aspectFill"></image>
				<text>这里是</text>
			</view>
			<view class="f2box2">
				<image src="../../static/img/adopt1.jpg" mode="aspectFill"></image>
				<text>这里是狗狗的</text>
			</view>
			<view class="f2box2">
				<image src="../../static/img/adopt1.jpg" mode="aspectFill"></image>
				<text>这里是狗狗的描述这里是狗狗的描述这里是狗狗的描述</text>
			</view>
	</view>
	</view>
	<!--  -->
</template>

<script>
	export default {
		data() {
			return {
				value: 0,
				range: [
					{ value: 0, text: "猫" },
					{ value: 1, text: "狗" },
					{ value: 2, text: "其他" },
				]
			}
		},
		methods: {
			change(e) {
			  console.log("e:", e);
			},
		}
	}
</script>

<style lang="scss">
	// F1
.f1box1{
	display: flex;
	>view{
		flex: 1;
	}
}
// F2
.f2box1{
	display: grid;
	grid-template-columns: repeat(2, 50%);
	.f2box2{
		display: flex;
		flex-direction: column;
		align-items: center;
		flex: 1;
		margin: 20rpx;
		box-shadow: 0 0 9px 3px #eeeeee;
		border-radius: 15rpx;
		>image{
			width: 300rpx;
			height: 330rpx;
			border-radius: 15rpx;
		}
		>text{
			width: 300rpx;
			display: block;
			margin-top: 10rpx;
			text-overflow: ellipsis;
			overflow: hidden;
			white-space: nowrap;
		}
	}
}
</style>
