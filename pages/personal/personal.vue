<template>
	<view class="bgColor" style="height: 100vh;">
		<view class="headerInformation">
			<view class="Information">
				<view class="name-gender-address">
					<image src="../../static/image/doctoring.png" mode="" class="doctoring"></image>
					<view class="">
						<view class="name-gender">
							<text class="name">张海淘</text>
							<image src="../../static/image/g.png" mode="" class="gender"></image>
							<text class="department">内科  主任医师</text>
						</view>
						<view class="address"><image src="../../static/image/address2.png" mode=""></image>重庆铭博互联网医院</view>
					</view>
				</view>
				<image src="../../static/image/certification.png" mode="" class="certificate"></image>
			</view>
			<view class="detail">
				<view class="">
					<text class="title">200</text>
					<text class="text">订单收入积分</text>
				</view>
				<view class="dbsob">
					<text class="title">500</text>
					<text class="text">处方收入积分</text>
				</view>
				<view class="">
					<text class="title">200</text>
					<text class="text">本月收入积分</text>
				</view>
			</view>
		</view>
		<view class="listPers">
			<view class="feiyong-arrow" @tap="wallet">
				<view class="feiyong">
					<image src="../../static/image/feiyong.png" mode=""></image>
					<text>我的钱包</text>
				</view>
				<image src="../../static/image/arrow.png" mode="" class="arrow"></image>
			</view>
			<view class="feiyong-arrow">
				<view class="feiyong">
					<image src="../../static/image/fuwu.png" mode=""></image>
					<text>服务设置</text>
				</view>
				<image src="../../static/image/arrow.png" mode="" class="arrow"></image>
			</view>
			<view class="feiyong-arrow" @tap="prescription">
				<view class="feiyong">
					<image src="../../static/image/xinwen.png" mode=""></image>
					<text>处方记录</text>
				</view>
				<image src="../../static/image/arrow.png" mode="" class="arrow"></image>
			</view>
			<view class="feiyong-arrow" @tap="professional">
				<view class="feiyong">
					<image src="../../static/image/professional.png" mode=""></image>
					<text>职业点管理</text>
				</view>
				<image src="../../static/image/arrow.png" mode="" class="arrow"></image>
			</view>
			<view class="feiyong-arrow" @tap="thenPhrase">
				<view class="feiyong">
					<image src="../../static/image/zixuntousu.png" mode=""></image>
					<text>常用语</text>
				</view>
				<image src="../../static/image/arrow.png" mode="" class="arrow"></image>
			</view>
			<view class="feiyong-arrow" @tap="system">
				<view class="feiyong">
					<image src="../../static/image/shezhi.png" mode=""></image>
					<text>系统设置</text>
				</view>
				<image src="../../static/image/arrow.png" mode="" class="arrow"></image>
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
			wallet() {
				/**
				 * 我的钱包
				 */
				uni.navigateTo({
				    url: '/pages/personal/wallet/index'
				});
			},
			system() {
				uni.navigateTo({
				    url: '/pages/personal/system/index'
				});
			},
			professional() {
				uni.navigateTo({
				    url: '/pages/personal/professional/index'
				});
			},
			thenPhrase() {
				uni.navigateTo({
				    url: '/pages/personal/thePhrase/index'
				});
			},
			prescription() {
				uni.navigateTo({
					url: '/pages/personal/prescription/index'
				});
			}
		}
	}
</script>

<style>
.headerInformation{
	background-color: #FFFFFF;
	margin:20upx 0;
}
.headerInformation .doctoring{
	width: 111upx;
	height: 111upx;
	margin-right: 26upx;
}
.headerInformation .certificate{
	width: 170upx;
	height: 128upx;
}
.Information{
	display: flex;
	justify-content: space-between;
	padding: 20upx 0 20upx 30upx;
}
.name-gender-address{
	display: flex;
	align-items: center;
}
.name-gender-address .gender{
	width: 20upx;
	height: 34upx;
	margin: 0 18upx;
}
.name-gender-address  .address{
	font-size: 28upx;
	color: #333333;
}
.name-gender-address  .address image{
	width: 22upx;
	height: 26upx;
	margin-right: 10upx;
}
.name-gender{
	margin-bottom: 10upx;
	color: #333333;
}
.name-gender .name{
	font-size: 34upx;
}
.name-gender .department{
	font-size: 28upx;
}
.detail{
	display: flex;
	justify-content: space-around;
	padding: 30upx 0;
}
.detail .dbsob{
	border-left: 1upx solid #dddddd;
	border-right: 1upx solid #dddddd;
}
.detail view{
	display: flex;
	flex-direction: column;
	align-items: center;
	width: 100%;
}
.detail .title{
	font-size: 44upx;
	color: #4d9dff;
}
.detail .text{
	font-size: 26upx;
	color: #333333;
	margin-top: 10upx;
}
</style>
