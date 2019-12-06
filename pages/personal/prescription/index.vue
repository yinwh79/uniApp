<template>
	<view class="bgColor he">
		<view class="prescript">
			<view class="list">
				<view class="header">
					<text class="bh">处方编号  yp7784351166</text>
					<text class="start">审核失败</text>
				</view>
				<view class="bodys">
					<view class="li">
						<text>患者：</text>
						<view>李晓楠</view>
					</view>
					<view class="li">
						<text>诊断：</text>
						<view>高血压</view>
					</view>
					<view class="li">
						<text>药品：</text>
						<view>将卡可代购；阿姨官方雕胶囊；更会发生喷剂；u发哈苏俄过打飞胶囊；合肥市当局否认冲剂</view>
					</view>
				</view>
			</view>
			<view class="list">
				<view class="header">
					<text class="bh">处方编号  yp7784351166</text>
					<text class="">已购买</text>
				</view>
				<view class="bodys">
					<view class="li">
						<text>患者：</text>
						<view>李晓楠</view>
					</view>
					<view class="li">
						<text>诊断：</text>
						<view>高血压</view>
					</view>
					<view class="li">
						<text>药品：</text>
						<view>将卡可代购；阿姨官方雕胶囊；更会发生喷剂；u发哈苏俄过打飞胶囊；合肥市当局否认冲剂</view>
					</view>
				</view>
			</view>
			<view class="list">
				<view class="header">
					<text class="bh">处方编号  yp7784351166</text>
					<text class="gq">已过期</text>
				</view>
				<view class="bodys">
					<view class="li">
						<text>患者：</text>
						<view>李晓楠</view>
					</view>
					<view class="li">
						<text>诊断：</text>
						<view>高血压</view>
					</view>
					<view class="li">
						<text>药品：</text>
						<view>将卡可代购；阿姨官方雕胶囊；更会发生喷剂；u发哈苏俄过打飞胶囊；合肥市当局否认冲剂</view>
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
				
			}
		},
		methods: {
			
		}
	}
</script>

<style>
.prescript{
	margin-top: 30upx;
}
.prescript .list{
	margin-bottom: 30upx;
	padding: 0 25upx;
	box-shadow:0px 0px 6px #ededed;
}
.prescript .list .header{
	height: 79upx;
	border-bottom: 1upx solid #e4e4e4;
	background-color: #cfe8fe;
	border-radius: 20upx 20upx 0 0;
	display: flex;
	justify-content: space-between;
	align-items: center;
	font-size: 34upx;
	padding: 0 20upx;
	color: #4b9cff;
}
.prescript .list .header .start{
	color: #bd0000;
}
.prescript .list .header .gq{
	color: #999999;
}
.prescript .list .bodys{
	background-color: #FFFFFF;
	border-radius: 0 0 20upx 20upx;
	padding: 38upx 20upx;
}
.prescript .list .bodys .li{
	font-size: 28upx;
	display: flex;
	margin-bottom: 5upx;
}
.prescript .list .bodys .li text{
	width: 100upx;
	flex-shrink: 0;
	color: #333333;
}
.prescript .list .bodys .li view{
	color: #999999;
}
</style>
