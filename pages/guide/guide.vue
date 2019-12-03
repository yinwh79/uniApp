<template>
	<view class="bgColor">
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
						<text>2</text>
					</view>
					<text class="t">证件上传</text>
				</view>
				<view class="tog">
					<image src="../../static/image/steps.png" mode=""></image>
				</view>
				<view class="cent">
					<view class="tex">
						<text>3</text>
					</view>
					<text class="t">认证成功</text>
				</view>
			</view>
		</view>
		<view class="identity colors">
			<label class="head">
				<view>
					<text></text>
					身份证
				</view>
			</label>
			<view class="idet">
				<label class="positive">
					<view class="idetOrd">
						<image src="../../static/image/positive.png" mode=""></image>
					</view>
					<view class="text-areas">拍摄正面</view>
				</label>
				<label class="reverse">
					<view class="idetOrd">
						<image src="../../static/image/reverse.png" mode=""></image>
					</view>
					<view class="text-areas">拍摄反面</view>
				</label>
			</view>
		</view>
		<view class="identity colors">
			<label class="head">
				<view>
					<text></text>
					执业证
				</view>
			</label>
			<view class="idet">
				<label class="positive">
					<view class="idetOrd">
						<image src="../../static/image/certificate.png" mode=""></image>
					</view>
					<view class="text-areas">上传证书</view>
				</label>
				<label class="reverse">
					<view class="idetOrd">
						<image src="../../static/image/certificate.png" mode=""></image>
					</view>
					<view class="text-areas">上传证书</view>
				</label>
			</view>
		</view>
		<view class="identity colors">
			<label class="head">
				<view>
					<text></text>
					个人简介
				</view>
			</label>
			<view class="Introduction">
				<textarea class="textAre"/>
			</view>
		</view>
		<view class="identity colors">
			<label class="head">
				<view>
					<text></text>
					擅长疾病
				</view>
			</label>
			<view class="Introduction">
				<textarea class="textAre"/>
			</view>
		</view>
		<view class="textNext">
			<!-- 只能用到微信小程序中 -->
			<!--#ifdef MP-WEIXIN-->
			<button type="button" class="loguin" @tap="nextPag">提交</button>
			 <!-- #endif -->
			 <!--除微信小程序平台其它平台都可以用 -->
			 <!--#ifndef MP-WEIXIN-->
			 <button type="primary" @tap="nextPag">提交</button>
			 <!-- #endif -->
		</view>
		<view class="skip">跳过></view>
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
			uni.navigateTo({
			    url: '/pages/guide/success',
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
.colors{
	background-color: #FFFFFF;
	margin-bottom: 20upx;
}
.colors .head{
	border-bottom: 1upx solid #e4e4e4;
	height: 86upx;
	line-height: 86upx;
	display: flex;
}
.colors .head view{
	font-size: 32upx;
	color: #333333;
	margin-left: 33upx;
}
.colors .head view text{
	border-left: 6upx solid #4d9dff;
	margin-right: 30upx;
}
.identity{
	
}
.identity .idet{
	display: flex;
	justify-content:space-between;
	padding:30upx;
}
.identity .idet image{
	width: 222upx;
	height: 148upx;
}
.identity .idet .idetOrd{
	width: 330upx;
	height: 220upx;
	background-color:#ecf5ff;
	display: flex;
	justify-content: center;
	align-items: center;
	border-radius: 20upx 20upx 0 0;
}
.identity .idet .text-areas{
	text-align: center;
	font-size: 28upx;
	color: #FFFFFF;
	background-color: #4d9dff;
	border-radius: 0 0 20upx 20upx;
	height: 60upx;
	line-height: 60upx;
}
.Introduction{
	padding: 40upx;
}
.textAre{
	width:100%;
	height: 200upx;
	background-color: #f1f1f1;
	border-radius:10upx;
	padding: 10upx;
}
.textNext{
	margin-top: 98upx;
	padding: 0 40upx;
}
.skip{
	color:#4d9dff;
	font-size: 32upx;
	text-align: center;
	padding: 20upx 0 40upx;
}
</style>
