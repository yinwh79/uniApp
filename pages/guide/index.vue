<template>
	<view>
		<view class="headers">
			<view class="bodys">
				<view class="cent xuanz">
					<view class="tex">
						<text>1</text>
					</view>
					<text class="t">基本信息</text>
				</view>
				<view class="tog">
					<image src="../../static/image/steps.png" mode=""></image>
				</view>
				<view class="cent">
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
		<view class="">
			<view class="upImages" @click="updataImg">
				<image src="../../static/image/upimage.png" mode=""></image>
				<text>上传头像</text>
			</view>
			<view class="Fillinthe">
				<view class="formRes bordTop">
					<view class="contents">
						<text class="col">*</text>
						<text class="texts">姓&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;名</text>
					</view>
					<input type="text" value="" placeholder="请输入真实姓名" placeholder-style="color:#e4e4e4"/>
				</view>
				<view class="formRes">
					<view class="contents">
						<text class="col">*</text>
						<text class="texts">在职医院</text>
					</view>
					<view class="uni-list-cell-db">
					<picker @change="bindPickerChange" :value="index" :range="array" class="pickes">
						<view class="uni-input">{{array[index]}}</view>
					</picker>
				    </view>
				</view>
				<view class="formRes">
					<view class="contents">
						<text class="col">*</text>
						<text class="texts">所在科室</text>
					</view>
					<input type="text" value="" placeholder="请输入真实姓名" placeholder-style="color:#e4e4e4"/>
				</view>
				<view class="formRes">
					<view class="contents">
						<text class="col">*</text>
						<text class="texts">临床职称</text>
					</view>
					<input type="text" value="" placeholder="请输入真实姓名" placeholder-style="color:#e4e4e4"/>
				</view>
				<view class="formRes">
					<view class="contents">
						<text class="col">*</text>
						<text class="texts">身份证号</text>
					</view>
					<input type="text" value="" placeholder="请输入你的身份证号号码" placeholder-style="color:#e4e4e4"/>
				</view>
				<view class="nextText">若没有您所在的医院及科室请联系客服400-123456</view>
				<view class="textNext">
					<!-- 只能用到微信小程序中 -->
					<!--#ifdef MP-WEIXIN-->
					<button type="button" class="loguin" @tap="nextPag">下一步</button>
					 <!-- #endif -->
					 <!--除微信小程序平台其它平台都可以用 -->
					 <!--#ifndef MP-WEIXIN-->
					 <button type="primary" @tap="nextPag">下一步</button>
					 <!-- #endif -->
				</view>
			</view>
		</view>
	</view>
</template>

<script>
import QSPickerCustom from '@/components/QS-inputs-split/elements/QS-picker-custom/index.vue';
export default {
	data() {
		return {
			picker_date: [],
			form: {
				picker_date: ''
			}
		}
	},
	components: {
		QSPickerCustom
	},
	methods: {
		updataImg() {
			uni.chooseImage({
				success: (chooseImageRes) => {
					const tempFilePaths = chooseImageRes.tempFilePaths;
					uni.uploadFile({
						url: 'https://www.example.com/upload', //仅为示例，非真实的接口地址
						filePath: tempFilePaths[0],
						name: 'file',
						formData: {
							'user': 'test'
						},
						success: (uploadFileRes) => {
							console.log(uploadFileRes.data);
						}
					});
				}
			});
		},
		nextPag() {
			uni.navigateTo({
			    url: '/pages/guide/guide',
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
.upImages{
	display: flex;
	flex-direction: column;
	align-items: center;
	margin:30upx 0;
}
.upImages image{
	width: 183upx;
	height: 183upx;
}
.upImages text{
	font-size: 28upx;
	color: #4d9dff;
	margin-top: 30upx;
}
.Fillinthe{
	padding: 0 22upx;
}
.Fillinthe .bordTop{
	border-top: 1upx solid #e5e5e5;
}
.Fillinthe .formRes{
	display: flex;
	height: 100upx;
	border-bottom: 1upx solid #e5e5e5;
	align-items: center;
}
.Fillinthe .formRes .contents{
	width: 180upx;
}
.Fillinthe .formRes .col{
	color: #e60012;
	font-size: 30upx;
	padding-left: 17upx;
	margin-right: 10upx;
}
.Fillinthe .formRes .texts{
	font-size: 30upx;
	color: #4a4a4a;
}
.uni-list-cell-db{
	width: 504upx;
}
.pickes{
	width: 100%;
}
.nextText{
	margin-top: 100upx;
	font-size: 26upx;
	color: #999999;
	padding-bottom: 20upx;
}
</style>
