<template>
	<view class="">
		<FuiNavBar class="bg-blue"> 
			<block slot="title">边框阴影</block>
		</FuiNavBar>
		<view class="wrap">
			<!-- 阴影 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/czdq.png" mode=""></image>
					阴影
				</view>

				<view class="fui-car__content padding-sm margin-xs">
					<view class="flex justify-content padding-tb-df margin-bottom-sm align-center shadow radius">
						默认高光阴影
					</view>
					<view class="flex justify-content padding-tb-xl margin-bottom-sm bg-blue align-center shadow-blur radius">
						<view class="center">
							根据颜色而改变的阴影
						</view>
					</view>

					<view class="flex justify-content padding-tb-xl margin-bottom-sm align-center shadow-blur radius" style="background-image: url(../../static/images/icons/shadow-bg.png);
	background-position: center;">
						<view class="center" style="color: #ffffff">
							根据背景图而改变的阴影
						</view>
					</view>
				</view>
			</view>
			<!-- 阴影 end -->
		</view>
	</view>
</template>

<script>
	import FuiNavBar from '@/common/FuiNavBar.vue'
	export default {
		components: {
			FuiNavBar
		}
	}
</script>

<style>
</style>
