<template>
	<view class="he headers" style="background-color: #FFFFFF;">
		<view class="phed">
			<view class="bodys">
				<view class="cent xuanz">
					<view class="tex">
						<image src="../../../../static/image/comp.png" mode=""></image>
					</view>
					<text class="t">密码验证</text>
				</view>
				<view class="tog">
					<image src="../../../../static/image/compTo.png" mode=""></image>
				</view>
				<view class="cent xuanz">
					<view class="tex">
						<image src="../../../../static/image/comp.png" mode=""></image>
					</view>
					<text class="t">修改密码</text>
				</view>
				<view class="tog">
					<image src="../../../../static/image/compTo.png" mode=""></image>
				</view>
				<view class="cent xuanz">
					<view class="tex">
						<text>3</text>
					</view>
					<text class="t">修改成功</text>
				</view>
			</view>
		</view>
		<view class="successIndex">
			<image src="../../../../static/image/after.png" mode=""></image>
			<view class="Congratulations">
				<text class="ations">恭喜您!</text>
				<text class="Congratu">账号更换成功</text>
			</view>
		</view>
		<view class="textNext">
			<!-- 只能用到微信小程序中 -->
			<!--#ifdef MP-WEIXIN-->
			<button type="button" class="loguin" @tap="nextPag">进入首页<text style="font-size: 28upx;">(3秒后自动跳转)</text></button>
			 <!-- #endif -->
			 <!--除微信小程序平台其它平台都可以用 -->
			 <!--#ifndef MP-WEIXIN-->
			 <button type="primary" @tap="nextPag">进入首页<text style="font-size: 28upx;">(3秒后自动跳转)</text></button>
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
			nextPag() {
				uni.switchTab({
				    url: '/pages/personal/personal'
				});
			}
		}
	}
</script>

<style>
	.phed{
		border-bottom: 20upx solid #f5f5f5;
		border-top: 20upx solid #f5f5f5;
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
.headers .bodys .tex image{
	width: 37upx;
	height: 26upx;
}
.textNext{
	position: absolute;
	bottom: 200upx;
	width: 90%;
	margin: 0 auto;
	left: 0;
	right: 0;
}
.pws{
	display: flex;
	justify-content: space-between;
	align-items: center;
	margin: 0 30upx;
	padding: 0 10upx;
	border-bottom: 1upx solid #e5e5e5;
	height:100upx;
}
.pws .ckpws{
	width: 41upx;
	height: 31upx;
}
.pws .possow{
	display: flex;
	align-items: center;
	font-size: 30upx;
	color: #4a4a4a;
}
.pws .possow .solids{
	border-right: 1upx solid #e5e5e5;
}
.pws .possow text{
	width: 100upx;
	display: inline-block;
}
.pws .possow input{
	margin-left: 20upx;
}
.dynamicCode .Codes{
	border: 1px solid #4d9dff;
	border-radius: 10upx;
	font-size: 30upx;
	color: #4d9dff;
	width: 189upx;
	height: 54upx;
	display: flex;
	justify-content: center;
	align-items: center;
}
.successIndex{
	display: flex;
	align-items: center;
	flex-direction: column;
}
.successIndex image{
	width: 177upx;
	height: 180upx;
	margin-top: 128upx;
}
.successIndex .ations{
	font-size: 40upx;
	color: #4a4a4a;
	padding-top: 63upx;
	display: flex;
	flex-direction: column;
	align-items: center;
}
.successIndex .Congratu{
	font-size: 36upx;
	color: #4a4a4a;
}
</style>
