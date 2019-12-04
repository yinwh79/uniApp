<template>
	<view class="bgColor" style="height: 100vh;overflow: hidden;">
		<view class="groupList">
			<view class="list" @tap="details()">
				<view class="title-alert">
					<text class="title">糖尿病（12人）</text>
					<text class="alert">李晓彤  林一朵  是你的风格  巍峨健  啊师傅  就啊师...</text>
				</view>
				<image src="../../static/image/jiant.png" mode="" class="gd"></image>
			</view>
			<view class="list" @tap="details()">
				<view class="title-alert">
					<text class="title">肠胃疾病（8人）</text>
					<text class="alert">李晓彤  林一朵  是你的风格  巍峨健  啊师傅  就啊师...</text>
				</view>
				<image src="../../static/image/jiant.png" mode="" class="gd"></image>
			</view>
			<view class="list" @tap="details()">
				<view class="title-alert">
					<text class="title">糖尿病（12人）</text>
					<text class="alert">李晓彤  林一朵  是你的风格  巍峨健  啊师傅  就啊师...</text>
				</view>
				<image src="../../static/image/jiant.png" mode="" class="gd"></image>
			</view>
		</view>
		<view class="textNext">
			<!-- 只能用到微信小程序中 -->
			<!--#ifdef MP-WEIXIN-->
			<button type="button" class="loguin" @tap="nextPag">添加分组</button>
			 <!-- #endif -->
			 <!--除微信小程序平台其它平台都可以用 -->
			 <!--#ifndef MP-WEIXIN-->
			 <button type="primary" @tap="nextPag">添加分组</button>
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
				uni.navigateTo({
				    url: '/pages/patients/addGroup'
				});
			},
			details() {
				uni.navigateTo({
				    url: '/pages/patients/grouping'
				});
			}
		}
	}
</script>

<style>
.textNext{
	padding: 0 40upx;
	margin-top: 100upx;
}
.groupList{
	background-color: #FFFFFF;
	margin-top: 30upx;
}
.groupList .gd{
	width: 16upx;
	height: 27upx;
}
.groupList .list{
	margin: 0 30upx;
	display: flex;
	justify-content: space-between;
	align-items: center;
	height: 136upx;
	border-bottom: 1upx solid #e4e4e4;
}
.groupList .list:last-child{
	border-bottom: none;
}
.groupList  .list .title{
	font-size: 32upx;
	color: #333333;
}
.groupList  .title-alert{
	display: flex;
	flex-direction: column;
}
.groupList  .list .alert{
	color: #dddddd;
	font-size: 26upx;
	margin-top: 10upx;
	white-space: nowrap;
	overflow: hidden;
	text-overflow: ellipsis;
}
</style>
