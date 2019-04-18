<template>
	<view class="content">
		<view>
			<view class="top">
				<text>通讯录</text>
				<image src="../../static/cha.png" class="top-c"></image>
			</view>
			<view class="top2">
				<button type="default" class="tong">
					<image src="../../static/user3.jpg" mode="circle"></image>刘磊
				</button>



				<button type="default" class="tong">
					<image src="../../static/user2.jpg" mode="circle"></image>朱林杰
				</button>



				<button type="default" class="tong">
					<image src="../../static/user1.jpg" mode="circle"></image>朱芮林
				</button>

				<!-- <view class="row" v-for="hand in date1">
				<view class="tong" >
					<text>{{hand.date1}}</text>
				</view>
				
				</view> -->
			</view>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				title: '朱林杰',
				/* date1:[
					{
						name:'好友'
					}
				] */
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
		height: 1150upx;
		background-color: #EEEEEE;
	}

	.top {
		margin-top: 60upx;
		height: 46upx;
		font-size: 36upx;
		width: 100%;
		display: flex;
		justify-content: space-between;
		background-color: #EEEEEE;

	}

	.top2 image {
		width: 100upx;
		height: 100upx;
	}

	.top-c {
		width: 35upx;
		height: 35upx;
		margin-right: 8upx;
	}

	.tong {
		display: flex;
		font-size: 36upx;
		text-align: left;
		background-color: #EEEEEE;
		padding: 10upx 10upx 10upx 10upx;
		border: 1upx;
		border-radius: 10upx;


	}

	.tong-p {
		margin-left: 5upx;
	}
</style>
