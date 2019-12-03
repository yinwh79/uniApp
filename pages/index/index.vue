<template>
	<view class="content">
		<view class="header" :style="{backgroundImage:`url(${imageUrl})`}">
			<view class="doctorImage">
				<image src="../../static/image/doctorimg.png" class="doctimg" mode=""></image>
				<view class="basic">
					<view class="information">
						<text class="names">张海淘</text>
						<image src="../../static/image/xb.png" mode="" class="xb"></image>
						<text class="professional">内科  主任医师</text>
					</view>
					<view class="address">
						<image src="../../static/image/dizhi.png" mode="" class="dizhi"></image>
						<text>重庆铭博互联网医院</text>
					</view>
				</view>
			</view>
			<view class="datas">
				<view class="">
					<text class="title">200</text>
					<text class="title_text">订单积分</text>
				</view>
				<view class="bianx">
					<text class="clearbot"></text>
					<view class="">
						<text class="title">500</text>
						<text class="title_text">处方积分</text>
					</view>
					<text class="clearbot"></text>
				</view>
				<view class="">
					<text class="title">200</text>
					<text class="title_text">本月积分</text>
				</view>
			</view>
		</view>
		<view class="nav">
			<view class="">
				<view class="nav1">
					<image src="../../static/image/nav1.png" mode=""></image>
				</view>
				<text>邀请患者</text>
			</view>
			<view class="">
				<view class="nav2">
					<image src="../../static/image/nav2.png" mode=""></image>
				</view>
				<text>咨询服务</text>
			</view>
			<view class="">
				<view class="nav3">
					<image src="../../static/image/nav3.png" mode=""></image>
				</view>
				<text>处方管理</text>
			</view>
		</view>
		<view class="Uselist">
			<view class="list">
				<image src="../../static/image/listimg.png" mode="" class="headImage"></image>
				<view class="text">
					<view class="title">
						<view class="name-age">
							<text class="name">张小贝</text>
							<image src="../../static/image/n.png" mode="" class="gender"></image>
							<text class="age">40岁</text>
						</view>
						<text class="date">2019-8-11</text>
					</view>
					<view class="foot">
						<text>备注：发橘色份回忆啊说</text>
						<text class="numb">58</text>
					</view>
				</view>
			</view>
			<view class="list">
				<image src="../../static/image/listimg2.png" mode="" class="headImage"></image>
				<view class="text">
					<view class="title">
						<view class="name-age">
							<text class="name">王大锤</text>
							<image src="../../static/image/g.png" mode="" class="gender"></image>
							<text class="age">17岁</text>
						</view>
						<text class="date">2019-8-11</text>
					</view>
					<view class="foot">
						<text>备注：发橘色份回忆啊说</text>
						<text class="numb">58</text>
					</view>
				</view>
			</view>
			<view class="list">
				<image src="../../static/image/listimg3.png" mode="" class="headImage"></image>
				<view class="text">
					<view class="title">
						<view class="name-age">
							<text class="name">赵笑到</text>
							<image src="../../static/image/n.png" mode="" class="gender"></image>
							<text class="age">5岁</text>
						</view>
						<text class="date">2019-8-11</text>
					</view>
					<view class="foot">
						<text>备注：v不是当局复合弓iu为何日图二为过12122121123</text>
						<text class="numb">9</text>
					</view>
				</view>
			</view>
			<view class="list">
				<image src="../../static/image/listimg3.png" mode="" class="headImage"></image>
				<view class="text">
					<view class="title">
						<view class="name-age">
							<text class="name">张小贝</text>
							<image src="../../static/image/n.png" mode="" class="gender"></image>
							<text class="age">40岁</text>
						</view>
						<text class="date">2019-8-11</text>
					</view>
					<view class="foot">
						<text>备注：发橘色份回忆啊说</text>
						<text class="numb">58</text>
					</view>
				</view>
			</view>
		</view>
	</view>
</template>

<script>
	import bgcoleorhead from '@/static/image/bgcoleorhead.png'
	export default {
		data() {
			return {
				imageUrl: bgcoleorhead,
				title: 'Hello'
			}
		},
		methods: {

		},
		onLoad() {
			const lst = false
			if (lst) {
				uni.navigateTo({
				    url: '/pages/guide/index'
				});
			}
		}
	}
</script>

<style>
.header{
	height:475upx ;
}
.doctorImage{
	display: flex;
	padding: 93upx 51upx 60upx;
	align-items: center;
}
.doctorImage .doctimg{
	width: 200upx;
	height: 200upx;
}
.doctorImage .basic{
	margin-left: 25upx;
	color: #FFFFFF;
}
.doctorImage .information{
	margin-bottom: 20upx;
}
.doctorImage .basic .names{
	font-size: 36upx;
}
.doctorImage .basic .professional{
	font-size: 32upx;
}
.doctorImage .basic .xb{
	width: 19upx;
	height: 34upx;
	margin: 0 30upx;
}
.doctorImage .address{
	font-size: 28upx;
}
.doctorImage .basic .dizhi{
	width: 21upx;
	height: 27upx;
	margin-right: 20upx;
}
.datas{
	margin: 0 22upx;
	border-radius: 20upx 20upx 0 0;
	height: 176upx;
	display: flex;
	justify-content: space-around;
	box-shadow:0px -2px 3px #DADDE3;
	background: -webkit-linear-gradient(top, #FFFFFF 60%,#eff6ff 100%) ;
}
.datas view{
	display: flex;
	flex-direction: column;
	align-items: center;
	justify-content: center;
	width: 100%;
}
.datas .bianx{
	display: flex;
	flex-direction: row;
	justify-content: space-between;
}
.datas .bianx .clearbot{
	width: 1px;
	height: 81upx;
	background-color: #cfe8ff;
}
.datas .title{
	font-size: 48upx;
	color: #2385fc;
}
.datas .title_text{
	font-size: 26upx;
	color: #aaaaaa;
}
.nav{
	display: flex;
	justify-content: space-around;
	margin-top: 95upx;
}
.nav .nav1,.nav .nav3,.nav .nav2{
	width: 120upx;
	height: 120upx;
	display: flex;
	justify-content: center;
	align-items: center;
	border-radius: 50%;
	margin-bottom: 18upx;
}
.nav .nav1{
	background-color: #558eff;
	box-shadow:3px 4px 18px #C2D7FF;
}
.nav .nav2{
	background-color: #009eff;
	box-shadow:3px 4px 18px #c5e6f9;
}
.nav .nav3{
	background-color: #767afd;
	box-shadow:3px 4px 18px #dfdffa;
}
.nav .nav1 image{
	width: 47upx;
	height: 58upx;
}
.nav .nav2 image{
	width: 58upx;
	height: 51upx;
	margin-right: 10upx;
}
.nav .nav3 image{
	width: 48upx;
	height: 51upx;
}
.nav text{
	color: #333333;
	font-size: 28upx;
}
.Uselist{
	margin:40upx 22upx 22upx;
}
.Uselist .list{
	display: flex;
	background: #ffffff;
	box-shadow:0px 0px 14px #EBF0F4;
	height: 136upx;
	align-items: center;
	padding: 0 22upx;
	border-radius: 20upx;
	margin-bottom: 20upx;
}
.Uselist .list .headImage{
	width: 91upx;
	height: 91upx;
	border-radius: 50%;
	flex-shrink: 0;
}
.Uselist .list .text{
	margin-left: 27upx;
	width: 100%;
}
.Uselist .list .foot{
	display: flex;
	justify-content: space-between;
}
.Uselist .list .foot text{
	font-size: 24upx;
	color: #aaaaaa;
	width: 400upx;
	overflow: hidden;
	text-overflow: ellipsis;
	-o-text-overflow: ellipsis;
	white-space:nowrap;
}
.Uselist .list .foot .numb{
	font-size: 20upx;
	color: #FFFFFF;
	background: #ff2500;
	width: 30upx;
	height: 30upx;
	border-radius: 50%;
	display: flex;
	justify-content: center;
	align-items: center;
}
.text .title{
	display: flex;
	justify-content: space-between;
	margin-bottom: 10upx;
}
.text .title .name{
	font-size: 30upx;
	color: #333333;
}
.text .title .age{
	font-size: 26upx;
	color: #333333;
}
.text .title .gender{
	width:16upx;
	height: 26upx;
	margin: 0 30upx;
}
.text .title  .date{
	font-size: 20upx;
	color: #aaaaaa;
}
</style>
