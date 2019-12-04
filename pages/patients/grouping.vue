<template>
	<view class="bgColor">
		<view class="addgroup">
			<text class="name">名称</text>
			<text>糖尿病</text>
		</view>
		<view class="groupLists">
			<view class="list">
				<image src="../../static/image/img03.png" mode="" class="headImg"></image>
				<view class="">
					<text class="name">刘娜</text>
					<image src="../../static/image/g.png" mode="" class="sex"></image>
					<text class="age">32岁</text>
				</view>
			</view>
			<view class="list">
				<image src="../../static/image/img04.png" mode="" class="headImg"></image>
				<view class="">
					<text class="name">李晓彤</text>
					<image src="../../static/image/g.png" mode="" class="sex"></image>
					<text class="age">32岁</text>
				</view>
			</view>
			<view class="list">
				<image src="../../static/image/img03.png" mode="" class="headImg"></image>
				<view class="">
					<text class="name">林一朵</text>
					<image src="../../static/image/g.png" mode="" class="sex"></image>
					<text class="age">32岁</text>
				</view>
			</view>
			<view class="list">
				<image src="../../static/image/img02.png" mode="" class="headImg"></image>
				<view class="">
					<text class="name">林二朵</text>
					<image src="../../static/image/g.png" mode="" class="sex"></image>
					<text class="age">32岁</text>
				</view>
			</view>
			<view class="list">
				<image src="../../static/image/img03.png" mode="" class="headImg"></image>
				<view class="">
					<text class="name">孟菲菲</text>
					<image src="../../static/image/g.png" mode="" class="sex"></image>
					<text class="age">32岁</text>
				</view>
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
			
		}
	}
</script>

<style>
	.bgColor{
		height: 100vh;
		overflow: hidden;
	}
.addgroup{
	background-color: #FFFFFF;
	height: 100upx;
	padding: 0 30upx;
	display: flex;
	align-items: center;
	margin-top: 30upx;
}
.addgroup .name{
	color:#999999 ;
	font-size: 32upx;
	margin-right: 30upx;
}
.groupLists{
	margin-top: 30upx;
}
.groupLists .list{
	display: flex;
	align-items: center;
	height: 140upx;
	background: #FFFFFF;
	padding: 0 30upx;
	border-bottom: 1upx solid #e4e4e4;
}
.groupLists .list:last-child{
	border-bottom: none;
}
.groupLists .name{
	color: #333333;
	font-size: 32upx;
}
.groupLists .age{
	font-size: 26upx;
	color: #333333;
}
.groupLists .sex{
	width: 17upx;
	height: 29upx;
	margin: 0 20upx;
}
.groupLists .headImg{
	width: 90upx;
	height: 90upx;
	margin-right: 40upx;
}
</style>
