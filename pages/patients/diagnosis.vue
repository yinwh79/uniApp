<template>
	<view class="bgColor" style="height: 100vh;">
		<view class="llist">
			<view class="patients">
				<view class="patients-title">
					<image src="../../static/image/img01.png" mode="" class="headImg"></image>
					<view class="">
						<view class="title">
							<text class="name">刘海海</text>
							<image src="../../static/image/n.png" mode="" class="sex"></image>
							<text class="age">40岁</text>
						</view>
						<text class="note">备注：阿斯顿把v</text>
					</view>
				</view>
				<text class="dataTime">2019-8-11</text>
			</view>
			<view class="patients">
				<view class="patients-title">
					<image src="../../static/image/img02.png" mode="" class="headImg"></image>
					<view class="">
						<view class="title">
							<text class="name">王陪陪</text>
							<image src="../../static/image/g.png" mode="" class="sex"></image>
							<text class="age">40岁</text>
						</view>
						<text class="note">备注：山东人钆额外</text>
					</view>
				</view>
				<text class="dataTime">2019-8-11</text>
			</view>
			
			<view class="patients">
				<view class="patients-title">
					<image src="../../static/image/img03.png" mode="" class="headImg"></image>
					<view class="">
						<view class="title">
							<text class="name">里邻</text>
							<image src="../../static/image/g.png" mode="" class="sex"></image>
							<text class="age">40岁</text>
						</view>
						<text class="note">备注：啊洞若观火有人问</text>
					</view>
				</view>
				<text class="dataTime">2019-8-11</text>
			</view>
			
			<view class="patients">
				<view class="patients-title">
					<image src="../../static/image/img04.png" mode="" class="headImg"></image>
					<view class="">
						<view class="title">
							<text class="name">江李彤</text>
							<image src="../../static/image/g.png" mode="" class="sex"></image>
							<text class="age">40岁</text>
						</view>
						<text class="note">备注：锕人特温柔体验</text>
					</view>
				</view>
				<text class="dataTime">2019-8-11</text>
			</view>
			
			<view class="patients">
				<view class="patients-title">
					<image src="../../static/image/img05.png" mode="" class="headImg"></image>
					<view class="">
						<view class="title">
							<text class="name">冉小贝</text>
							<image src="../../static/image/g.png" mode="" class="sex"></image>
							<text class="age">40岁</text>
						</view>
						<text class="note">备注：发橘色份回忆啊说</text>
					</view>
				</view>
				<text class="dataTime">2019-8-11</text>
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
.llist{
	background-color:#FFFFFF;
	margin-top: 30upx;
}
.patients{
	border-bottom: 1upx solid #e4e4e4;
	margin: 0 30upx;
	display: flex;
	justify-content: space-between;
	height: 144upx;
}
.patients .headImg{
	width: 90upx;
	height: 90upx;
	margin-right: 40upx;
}
.patients .sex{
	width: 17upx;
	height: 29upx;
	margin: 0 20upx;
}
.patients .patients-title{
	display: flex;
	align-items: center;
}
.patients .note{
	font-size: 24upx;
	color: #666666;
}
.patients .dataTime{
	font-size: 20upx;
	color: #999999;
	margin-top: 30upx;
}
.patients .title{
	font-size: 32upx;
	color: #333333;
}
.patients .age{
	font-size: 26upx;
	color: #333333;
}
</style>
