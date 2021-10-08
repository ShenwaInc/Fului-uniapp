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

<style lang="scss">
	/*每个页面公共css */
	@import url(@/common/css/main.scss);

	body {
		background-color: $uni-bg-color;
	}

	.foot {
		position: fixed;
		height: 130rpx;
		width: 100%;
		background-color: #fff;
		bottom: 0;
		box-shadow: 1px -1px 5px #e8e7e7;
		display: flex;
		justify-content: space-evenly;
		align-items: center;
	}

	.wrap {
		padding: 0 48rpx;
		width: 100%;

		/* 	height: calc(100vh - 218rpx); */
		.wrap-item {
			background-color: #FFF;
		}
	}

	.title {
		font-size: 68rpx;
		font-family: PingFangSC-Medium, PingFang SC;
		font-weight: 600;
		color: #060C24;
		line-height: 96rpx;
		padding-top: 62rpx;
		padding-bottom: 50rpx;

	}

	.nav-item {
		width: 302rpx;
		height: 150rpx;
	}

	.fui-icon {
		uni-image {
			width: 48rpx;
			height: 48rpx;
			margin-bottom: 13rpx;
		}
	}

	.icon-font {
		font-size: 11px;
		color: #A5AABB;
	}

	.nav-list {
		display: flex;
		justify-content: space-between;
		flex-wrap: wrap;
	}

	.nav-item {
		display: flex;
		border-radius: var(--fui-border-radius);
		background-color: white;
		box-shadow: 1px 1px 5px #e8e7e7;
		align-items: center;
		margin-bottom: 38rpx;

		.item-img {

			uni-image {
				width: 150rpx;
				height: 150rpx;
			}
		}

		.item-title {
			font-size: 34rpx;
			font-weight: 600;
			margin-bottom: 8rpx;
		}

		.item-text {
			font-size: 26rpx;
			font-weight: 400;
			color: #888;
		}
	}

	.extebdList {
		display: flex;
		flex-wrap: wrap;
		justify-content: space-around;

		.extebd-item {
			width: 310rpx;
			height: 310rpx;
			display: flex;
			flex-direction: column;
			justify-content: center;
			align-items: center;
			color: #FFF;
			margin-bottom: 18rpx;
			border-radius: var(--fui-border-radius);

			.extebd-title {
				font-size: 40rpx;
				margin-top: 10px;

			}

			.extebd-text {
				font-size: 28rpx;
				margin-top: 5px;

			}
		}
	}

	.about {
		background-image: url(./static/images/icons/about.png);
		height: 412rpx;
		background-size: contain;
		color: #FFFFFF;

		.wrap {
			.about-title {
				padding-top: 52rpx;
				font-size: 64rpx;
				font-style: italic;
			}

			.about-text {
				padding-top: 12rpx;
				font-size: 56rpx;
				font-style: italic;
			}

			.about-box {
				padding-top: 54rpx;
				display: flex;

				.box {
					margin-right: 100rpx;

					.box-title {
						font-size: 30rpx;
						color: #FF9C08;
						font-weight: 600;
					}

					.box-text {
						font-size: 28rpx;
					}
				}
			}

			.abouList {
				background-color: #fff;
				height: 480rpx;
				width: inherit;
				padding-top: 8px;
				padding-bottom: 8px;
				border-radius: var(--fui-border-radius);

				.about-item {
					display: flex;
					color: #333;
					height: 110rpx;
					align-items: center;

					uni-image {
						width: 34rpx;
						height: 34rpx;
						margin-left: 60rpx;
					}



					.about-item-text {
						margin-left: 40rpx;
						font-size: 30rpx;
						flex: 1;
						padding: 34rpx 0;
						position: relative;

						&::after {
							content: '';
							display: block;
							width: 100%;
							border-bottom: 4rpx solid #F0F0F0;
							position: absolute;
							bottom: 0;

						}
					}

				}

				.about-item:last-child .about-item-text::after {
					width: 0;
				}
			}
		}

	}


</style>
