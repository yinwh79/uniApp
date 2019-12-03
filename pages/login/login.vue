<template>
	<view class="bgColor logins">
		<view class="login">
			<view class="header">
				<text @tap="isShow = true" :class="isShow ? 'selected': ''">快速登陆</text>
				<text @tap="isShow = false" :class="!isShow ? 'selected': ''">账号密码登陆</text>
			</view>
			<view class="">
				<view class="" v-if="isShow">
					<view class="bodys">
						<view class="porn">
							<text>86+</text>
							<input type="text" value="" class="input" placeholder="请输入手机号" placeholder-style="color:#e4e4e4"/>
						</view>
						<view class="dynamic">
							<text class="title-text">验证码</text>
							<input type="text" value="" class="input" placeholder="请输入动态码" placeholder-style="color:#e4e4e4"/>
							<text class="mic">获取动态码</text>
						</view>
					</view>
					<view class="agreement">
						点击登录即同意<text>《铭博护理网医院用户注册协议》</text>
					</view>
					<view class="btn">
						<!-- 只能用到微信小程序中 -->
						<!--#ifdef MP-WEIXIN-->
						<button type="button" class="loguin" @tap="openIndex">登陆</button>
						 <!-- #endif -->
						 <!--除微信小程序平台其它平台都可以用 -->
						 <!--#ifndef MP-WEIXIN-->
						 <button type="primary" @tap="openIndex">登陆</button>
						 <!-- #endif -->
					</view>
					<view class="Otherways">
						<text>其他方式登陆</text>
					</view>
					<view class="wxlogin">
						<image src="../../static/image/wx.png" mode=""></image>
						<text>微信登录</text>
					</view>
				</view>
				<view class="userLogin" v-else>
					<view class="bodys">
						<view class="porn">
							<text>86+</text>
							<input type="text" value="" class="input" placeholder="请输入手机号" placeholder-style="color:#e4e4e4"/>
						</view>
						<view class="dynamic">
							<text class="title-text">密码</text>
							<input type="text" value="" class="input" placeholder="请输入密码" placeholder-style="color:#e4e4e4"/>
						</view>
					</view>
					<view class="btn useralog">
						<!-- 只能用到微信小程序中 -->
						<!--#ifdef MP-WEIXIN-->
						<button type="button" class="loguin" @tap="openIndex">登陆</button>
						 <!-- #endif -->
						 <!--除微信小程序平台其它平台都可以用 -->
						 <!--#ifndef MP-WEIXIN-->
						 <button type="primary" @tap="openIndex">登陆</button>
						 <!-- #endif -->
						 <text class="forgetpwd">忘记密码?</text>
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
				isShow: true,
			}
		},
		methods: {
			openIndex() {
				uni.switchTab({
				    url: '/pages/index/index',
				});
			}
		}
	}
</script>

<style scoped>
.bgColor{background: #f5f5f5;height: 100vh;}
.logins .login {
	padding:20upx 23upx;
}
.logins .header{
	display: flex;
}
.logins .header text{
	width: 50%;
	text-align: center;
	height: 100upx;
	line-height: 100upx;
	background-color:#dddddd;
	color: #333333;
	font-size: 32upx;
}
.logins .header text.selected{
	background-color:#4b9cff;
	color: #FFFFFF;
}
.logins .bodys{
	background-color: #FFFFFF;
	height:211upx;
	padding:0 28upx;
}
.logins .porn{
	display: flex;
	flex-direction: row;
	align-items: center;
	height: 107upx;
	border-bottom: 1upx solid #e5e5e5;
}
.logins .porn text{
	border-right: 1px solid #e5e5e5;
	color: #4a4a4a;
	height: 36upx;
	display: flex;
	align-items: center;
	padding-right: 22upx;
}
.logins .porn .input{
	margin-left: 40upx;
	width: 100%;
}
.logins .dynamic{
	display: flex;
	height: 107upx;
	justify-content: space-between;
	align-items: center;
}
.logins .title-text{
	color:#4a4a4a;
}
.logins .dynamic input{
	width: 300upx;
}
.logins .dynamic .mic{
	width:190upx;
	height: 55upx;
	border: 1upx solid #4a9cff;
	color: #4a9cff;
	font-size:30upx;
	border-radius: 10upx;
	display: flex;
	justify-content: center;
	align-items: center;
}
.logins .agreement{
	font-size: 26upx;
	color: #999999;
	padding:20upx 0;
}
.logins .agreement text{
	color: #4b9cff;
}
.logins .btn {
	margin-top:260upx;
}
.logins .btnClas{background-color: #4b9cff;}
.logins .Otherways{
	border-top: 1px solid #b3b3b3;
	margin-top: 100upx;
	display: flex;
	justify-content: center;
}
.logins .Otherways text{
	text-align: center;
	color: #333333;
	width: 250upx;
	position: relative;
	top: -26upx;
	background: #f5f5f5;
}
.logins .wxlogin{
	display: flex;
	flex-direction: column;
	align-items: center;
}
.logins .wxlogin image{
	width: 99upx;
	height: 99upx;
	margin: 30upx 0 20upx;
}
.logins .wxlogin text{
	color: #aaaaaa;
	font-size: 32upx;
}

.logins .userLogin .bodys .dynamic{
	justify-content: flex-start;
}
.logins .userLogin .bodys .dynamic .input{
	margin-left: 60upx;
}
.logins .useralog{
	margin-top: 500upx;
}
.logins .forgetpwd{
	font-size: 26upx;
	color: #2e95fd;
	display: flex;
	justify-content: flex-end;
	margin-top: 30upx;
}
</style>
