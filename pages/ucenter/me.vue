<template>
	<view class="content">
		<view class="item">
			<view class="head">
				<image :src="pic"></image>
			</view>
			<view class="message">
				<text class="title">{{name}}</text>
				<text class="WeChatId">{{WeChatId}}</text>
			</view>

		</view>
		<navigator url="setting" hover-class="navigator-hover">

			<view class="pay">
				<button type="default" class="bth">
					<image src="../../static/pay.png" mode="支付"></image>支付
				</button>
			</view>

			<view class="collect">
				<button type="collect" class="bth">
					<image src="../../static/collect.png" mode="收藏"></image>收藏
				</button>
			</view>

			<view class="ba">
				<button type="photo" class="bth">
					<image src="../../static/photo.png" mode="相册"></image>相册
				</button>
			</view>

			<view class="ba">
				<button type="card" class="bth">
					<image src="../../static/card.png" mode="卡包"></image>卡包
				</button>
			</view>

			<view class="ba">
				<button type="expression" class="bth">
					<image src="../../static/expression.png" mode="表情"></image>表情
				</button>
			</view>

			<view class="set">
				<button type="set" class="bth">
					<image src="../../static/set.png" mode="设置"></image>设置
				</button>
			</view>

		</navigator>


	</view>
</template>

<script>
	export default {
		data() {
			return {
				pic: '../../static/head.jpg',
				name: '1只念旧的兔子',
				WeChatId:   '微信号:162329560zny',
			}
		},
		onLoad() {

		},
		methods: {

		}
	}
</script>

<style>
	.content {
		text-align: center;
		height: 200upx;
	}

	.item {
		display: flex;
	}

	.message {
		display: flex;
		flex-direction: column;
		margin-left: 50upx;
	}

	.title {
		font-size: 36upx;
		margin-top: 20px;
	}

	.head image {
		width: 60px;
		height: 60px;
	       margin-left: 20upx;
		margin-top: 20upx;
	}

	.WeChatId {
		font-size: 30upx;
		color: #8F8F94;
	}

	.pay image {
		width: 23px;
		height: 23px;
		margin-right: 10px;
	}
	.pay{
		margin-top: 15upx;
	}
	.collect image {
		width: 23px;
		height: 23px;
		margin-right: 10px;
	}
	.collect{
		margin-top: 15upx;
	}

	.ba image {
		width: 23px;
		height: 23px;
		margin-right: 10px;
	}
	
	.set image {
		width: 23px;
		height: 23px;
		margin-right: 10px;
	}
       .set{
		margin-top: 15upx;
	}
	.bth {
		text-align: left;
	}
</style>
