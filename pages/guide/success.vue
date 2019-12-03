<template>
	<view>
		<view class="headers">
			<view class="bodys">
				<view class="cent xuanz">
					<view class="tex">
						<image src="../../static/image/comp.png" mode=""></image>
					</view>
					<text class="t">基本信息</text>
				</view>
				<view class="tog">
					<image src="../../static/image/compTo.png" mode=""></image>
				</view>
				<view class="cent xuanz">
					<view class="tex">
						<image src="../../static/image/comp.png" mode=""></image>
					</view>
					<text class="t">证件上传</text>
				</view>
				<view class="tog">
					<image src="../../static/image/compTo.png" mode=""></image>
				</view>
				<view class="cent xuanz">
					<view class="tex">
						<text>3</text>
					</view>
					<text class="t">认证成功</text>
				</view>
			</view>
		</view>
		<view class="after">
			<image src="../../static/image/after.png" mode=""></image>
			<text class="text1">恭喜您!</text>
			<text class="text2">账号更换成功</text>
		</view>
		<view class="textNext">
			<!-- 只能用到微信小程序中 -->
			<!--#ifdef MP-WEIXIN-->
			<button type="button" class="loguin" @tap="nextPag">进入首页<text>(3秒后自动跳转)</text></button>
			 <!-- #endif -->
			 <!--除微信小程序平台其它平台都可以用 -->
			 <!--#ifndef MP-WEIXIN-->
			 <button type="primary" @tap="nextPag">进入首页<text>(3秒后自动跳转)</text></button>
			 <!-- #endif -->
		</view>
	</view>
</template>

<script>
export default {
	data() {
		return {
			picker_date: [],
			form: {
				picker_date: ''
			}
		}
	},
	methods: {
		nextPag() {
			uni.switchTab({
			    url: '/pages/index/index'
			});
		}
	}
}
</script>

<style>
.headers{
	border-bottom: 20upx solid #f5f5f5;
	border-top: 20upx solid #f5f5f5;
	background-color: #ffffff;
}
.headers .bodys{
	display: flex;
	width: 80%;
	justify-content: space-between;
	align-items: center;
	padding: 20upx 0;
	margin: 0 auto;
}
.headers .bodys .tog{
	margin-top: -40upx;
}
.headers .bodys .tog image{width:100upx;height: 25upx;}
.headers .bodys text{font-size: 26upx;color:#a0a0a0 ;}
.headers .bodys .tex{
	border: 1px solid #cccccc;
	border-radius: 50%;
	width: 72upx;
	height: 72upx;
	font-size:48upx;
	display: flex;
	justify-content: center;
	align-items: center;
}
.headers .bodys .cent{
	display: flex;
	justify-content: center;
	align-items: center;
	flex-direction: column;
}
.headers .bodys .tex text{
	width: 60upx;
	height: 60upx;
	background-color: #cccccc;
	border-radius: 50%;
	text-align: center;
	line-height: 60upx;
	color: #FFFFFF;
	font-weight: bold;
	font-size: 48upx;
}
.headers .bodys .tex image{
	width: 37upx;
	height: 26upx;
}
.headers .bodys .t{
	margin-top: 10upx;
}
.headers .bodys .xuanz .tex{
	border: 1px solid #4d9dff;
}
.headers .bodys .xuanz .tex text{
	background-color: #4d9dff;
}
.headers .bodys .xuanz .t{
	color: #4d9dff;
}
.after{
	display: flex;
	flex-direction: column;
	align-items: center;
}
.after image{
	width: 178upx;
	height: 179upx;
	padding: 130upx 0 65upx;
	color: #4a4a4a;
}
.after .text1{
	font-size:40upx;
}
.after .text2{
	font-size:36upx;
}
.textNext{
	margin-top: 100upx;
	padding: 0 40upx;
}
.textNext text{
	font-size: 28upx;
	margin-left: 20upx;
}
</style>
