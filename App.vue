<script>
	export default {
		onLaunch: function() {
			console.log('App Launch')
		},
		onShow: function() {
			console.log('App Show')
		},
		onHide: function() {
			console.log('App Hide')
		}
	}
</script>

<style>
	/*每个页面公共css */
	*{-webkit-text-size-adjust: none;}
	.loguin{
		width: 100%;
		height: 100upx;
		display: flex;
		justify-content: center;
		align-items: center;
		text-align: center;
		background-color: #4b9cff;
		border-radius: 10upx;
		color: #FFFFFF;
	}
	.bgColor{
		background-color: #f5f5f5;
		overflow: hidden;
	}
	.he{
		height: 100vh;
	}
	.list-money {
		background-color: #FFFFFF;
		margin-top: 30upx;
	}
	.list-money .list{
		display: flex;
		justify-content: space-between;
		align-items: center;
		height: 100upx;
		margin: 0 30upx;
		border-bottom: 1upx solid #e4e4e4;
	}
	.list-money .gd{
		width: 16upx;
		height: 27upx;
	}
	/**
	 * 我的公共
	 */
	.listPers{
		background-color: #FFFFFF;
	}
	.listPers .feiyong-arrow{
		padding: 0 23upx;
		display: flex;
		justify-content: space-between;
		align-items: center;
		height: 100upx;
		border-bottom: 1upx solid #e4e4e4;
	}
	.listPers .feiyong{
		display: flex;
		align-items: center;
	}
	.listPers .feiyong text{
		font-size: 28upx;
		color: #4a4a4a;
	}
	.listPers .feiyong-arrow .feiyong image{
		width: 40upx;
		height: 40upx;
		margin-left: 13upx;
		margin-right: 40upx;
		flex-shrink:0;
	}
	.listPers .feiyong-arrow .arrow{
		width: 16upx;
		height: 27upx;
	}
</style>
