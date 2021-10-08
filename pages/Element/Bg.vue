<template>
	<view class="">
		<FuiNavBar>
			<block slot="content">背景</block>
		</FuiNavBar>
		<view class="wrap">
			<!-- 颜色 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/czdq.png" mode=""></image>
					颜色
				</view>
				<view class="fui-car__content padding-sm margin-xs">
					<view class="row square-3 justify-between font-xs">
						<view class="primary radius shadow-blur">
							<view class="center">
								基础色
								#0078d4
							</view>
						</view>
						<view class="error radius shadow-blur">
							<view class="center">
								错误提示色 #E8484C
							</view>
						</view>
						<view class="warning radius shadow-blur">
							<view class="center">
								警告色#574305
							</view>
						</view>
						<view class="primary radius light shadow-blur">
							<view class="center">
								浅基础色 #CCE6FF
							</view>
						</view>
						<view class="error radius light shadow-blur">
							<view class="center">
								浅错误提示色#FFF3F4
							</view>
						</view>
						<view class="warning radius light shadow-blur">
							<view class="center">
								浅警告色#E2DDCC
							</view>
						</view>
		
		
					</view>
				</view>
			</view>
			<!-- 颜色 end -->
			<!-- 中性色 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/zxs.png" mode=""></image>
					中性色
				</view>
				<view class="fui-car__content padding-sm margin-xs">
					<view class="row square-3 justify-between font-xs">
						<view class="bg-black radius shadow-blur">
							<view class="center">
								深黑色 #222222
							</view>
						</view>
						<view class="bg-darkgrey radius shadow-blur">
							<view class="center">
								深灰色 #777777
							</view>
						</view>
						<view class="bg-bg_grey radius shadow-blur">
							<view class="center">
								背景灰 #F1F1F1
							</view>
						</view>
						<view class="bg-font_grey radius shallow shadow-blur">
							<view class="center">
								字体灰#8e8e93
							</view>
						</view>
						<view class="bg-light_gray radius shallow shadow-blur">
							<view class="center">
								浅灰色#A8A8AC
							</view>
						</view>
						<view class="bg-border_gray radius shallow shadow-blur">
							<view class="center">
								边框灰#C8C8C8
							</view>
						</view>
						<view class="bg-border_light_gray radius shallow shadow-blur">
							<view class="center">
								边框浅灰#E1E1E1
							</view>
						</view>
						<view class="bg-bg_light_gray radius shallow shadow-blur">
							<view class="center">
								背景浅灰#F8F8F8
							</view>
						</view>
						<view class="bg-white radius shallow shadow-blur">
							<view class="center">
								背景白色#FFFFFF
							</view>
						</view>
					</view>
				</view>
			</view>
			<!-- 中性色 end -->
			<!-- 全局颜色 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/spdq.png" mode=""></image>
					颜色
				</view>
				<view class="fui-car__content padding-sm margin-xs">
					<view class="row square-3 justify-between font-xs">
						<view class="bg-maroon radius shadow-blur">
							<view class="center ">
								#750B1C
							</view>
						</view>
						<view class="bg-brown radius shadow-blur">
							<view class="center">
								#A4262C
							</view>
						</view>
						<view class="bg-red radius shadow-blur">
							<view class="center">
								#E0243A
							</view>
						</view>
						<view class="bg-tawny radius shadow-blur">
							<view class="center">
								#D67152
							</view>
						</view>
						<view class="bg-brown radius shadow-blur">
							<view class="center">
								#B33C24
							</view>
						</view>
						<view class="bg-green radius shadow-blur">
							<view class="center">
								#21A366
							</view>
						</view>
						
						<view class="bg-darkgreen radius shadow-blur">
							<view class="center">
								#005E50
							</view>
						</view>
						<view class="bg-teal radius shadow-blur">
							<view class="center">
								#038387
							</view>
						</view>
						<view class="bg-blue radius shadow-blur">
							<view class="center">
								#2C5EC2
							</view>
						</view>
						
						<view class="bg-royalblue radius shadow-blur">
							<view class="center">
								#004e8c
							</view>
						</view>
						<view class="bg-dodgerblue radius shadow-blur">
							<view class="center">
								#4f6bed
							</view>
						</view>
						<view class="bg-navy radius shadow-blur">
							<view class="center">
								#373277
							</view>
						</view>
						<view class="bg-purple radius shadow-blur">
							<view class="center">
								#7738B3
							</view>
						</view>
						<view class="bg-plum radius shadow-blur">
							<view class="center">
								#c239b3
							</view>
						</view>
						<view class="bg-pink radius shadow-blur">
							<view class="center">
								#e3008c
							</view>
						</view>
					</view>
				</view>
			</view>
			<!-- 全局颜色 end -->
		</view>
	</view>
</template>

<script>
	import FuiNavBar from '@/common/FuiNavBar';
	export default {
		components: {
			FuiNavBar
		},
		data() {
			return {

			}
		}
	}
</script>

<style>
</style>
