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
	}
</style>
