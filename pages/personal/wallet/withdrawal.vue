<template>
	<view class="bgColor he">
		<view class="listPers withdra">
			<view class="feiyong-arrow" @tap="failedWithdraw">
				<view class="feiyong">
					<image src="../../../static/image/audit.png" mode=""></image>
					<view class="time-describe">
						<text class="time">2018-08-30  17:20</text>
						<text class="describe">审核描述：待审核</text>
					</view>
				</view>
				<view class="rightM">
					<text>－30.00</text>
					<image src="../../../static/image/arrow.png" mode="" class="arrow"></image>
				</view>
			</view>
			<view class="feiyong-arrow" @tap="failedWithdraw">
				<view class="feiyong">
					<image src="../../../static/image/errors.png" mode=""></image>
					<view class="time-describe">
						<text class="time">2018-08-30  17:20</text>
						<text class="describe">审核描述：审核失败</text>
					</view>
				</view>
				<view class="rightM">
					<text>－30.00</text>
					<image src="../../../static/image/arrow.png" mode="" class="arrow"></image>
				</view>
			</view>
			<view class="feiyong-arrow" @tap="failedWithdraw">
				<view class="feiyong">
					<image src="../../../static/image/transfer.png" mode=""></image>
					<view class="time-describe">
						<text class="time">2018-08-30  17:20</text>
						<text class="describe">审核描述：待转账</text>
					</view>
				</view>
				<view class="rightM">
					<text>－30.00</text>
					<image src="../../../static/image/arrow.png" mode="" class="arrow"></image>
				</view>
			</view>
			<view class="feiyong-arrow" @tap="HaveTransfer">
				<view class="feiyong">
					<image src="../../../static/image/successs.png" mode=""></image>
					<view class="time-describe">
						<text class="time">2018-08-30  17:20</text>
						<text class="describe">审核描述：已提现</text>
					</view>
				</view>
				<view class="rightM">
					<text>－30.00</text>
					<image src="../../../static/image/arrow.png" mode="" class="arrow"></image>
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
			/**
			 * 未能提现
			 */
			failedWithdraw() {
				uni.navigateTo({
				    url: '/pages/personal/wallet/failedWithdraw'
				});
			},
			/**
			 * 成功提现
			 */
			HaveTransfer() {
				uni.navigateTo({
				    url: '/pages/personal/wallet/successfulWithdrawal'
				});
			}
		}
	}
</script>

<style>
.withdra{
	margin-top: 30upx;
	
}
.withdra .feiyong-arrow{
	height: 110upx;
}
.withdra .feiyong-arrow:last-child{
	border-bottom: none;
}
.withdra .time-describe {
	display: flex;
	flex-direction: column;
}
.withdra .time-describe .time{
	font-size: 32upx;
	color: #333333;
}
.withdra .time-describe .describe{
	font-size: 26upx;
	color: #cccccc;
}
.withdra .rightM text{
	margin-right: 20upx;
	color: #fc2702;
	font-size: 28upx;
}
</style>
