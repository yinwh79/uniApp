<template>
	<view class="bgColor he">
		<view class="binding">
			<view class="list">
				<text class="title">姓  名</text>
				<text class="text">张林云</text>
			</view>
			<view class="list">
				<text class="title">卡  号</text>
				<text class="text">621704098762536471</text>
			</view>
			<view class="list">
				<text class="title">银  行</text>
				<view class="right">
					<view class="right-titles">
						<image src="../../../static/image/zsyyhk.png" mode="" style="width: 55upx;height: 55upx;flex-shrink: 0;"></image>
						<view class="titles">
							<text class="names">招商银行</text>
							<text class="yh">储蓄卡</text>
						</view>
					</view>
					<image src="../../../static/image/arrow.png" mode="" class="arrows"></image>
				</view>
			</view>
			<view class="list">
				<text class="title">身份证</text>
				<text class="text">5338544587268986</text>
			</view>
		</view>
		<view class="tel">
			<view class="list">
				<text class="title">手机号</text>
				<text>+86 136****6587</text>
			</view>
			<view class="list">
				<text class="title">验证码</text>
				<view class="yzm">
					<input type="text" value="" placeholder="短信验证码" placeholder-style="color:#bbbbbb;"/>
					<view class="getyzm">
						<text>获取验证码</text>
					</view>
				</view>
			</view>
		</view>
		<view class="textNext">
			<!-- 只能用到微信小程序中 -->
			<!--#ifdef MP-WEIXIN-->
			<button type="button" class="loguin" @tap="binding">确认绑定</button>
			 <!-- #endif -->
			 <!--除微信小程序平台其它平台都可以用 -->
			 <!--#ifndef MP-WEIXIN-->
			 <button type="primary" @tap="binding">确认绑定</button>
			 <!-- #endif -->
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
			binding() {
				uni.navigateBack({
				    delta: 1
				});
			}
		}
	}
</script>

<style>
.textNext{
	width: 90%;
	margin: 0 auto;
	margin-top: 300upx;
}
.binding{
	background-color: #FFFFFF;
	margin-top: 30upx;
}
.binding .list{
	display: flex;
	border-bottom: 1upx solid #e8e8e8;
	height: 100upx;
	align-items: center;
}
.binding .list .right{
	display: flex;
	align-items: center;
	justify-content: space-between;
	width: 100%;
	flex-direction: row;
}
.binding .list .title{
	width: 150upx;
	text-align: center;
	display: inline-block;
	color: #333333;
	font-size: 32upx;
}
.binding .list .right .titles{
	font-size: 32upx;
	color: #333333;
}
.binding .list .right .names{
	padding: 0 20upx;
}
.binding .list .right .yh{
	color: #999999;
	font-size: 28upx;
}
.binding .list .right .right-titles{
	display: flex;
	flex-direction: row;
	align-items: center;
}
.binding .list .right .arrows{
	margin-right: 30upx;
}
.tel{
	margin-top: 30upx;
	background: #FFFFFF;
}
.tel .list{
	display: flex;
	align-items: center;
	height: 100upx;
	border-bottom: 1upx solid #e8e8e8;
	padding: 0 30upx;
	font-size: 32upx;
	color: #333333;
}
.tel .list:last-child{
	border-bottom:none;
}
.tel .list .title{
	width: 130upx;
}
.tel .list .yzm{
	display: flex;
	justify-content: space-between;
	align-items: center;
}
.tel .list .yzm .getyzm{
	width: 186upx;
	height: 56upx;
	border:1upx solid #4d9dff;
	border-radius: 10upx;
	display: flex;
	justify-content: center;
	align-items: center;
	color: #4d9dff;
	font-size: 28upx;
}

</style>
