<template>
	<view class="">
		<FuiNavBar class="bg-blue"> 
			<block slot="title">加载</block>
		</FuiNavBar>
		<view class="wrap">
			<!-- 加载状态 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/gdcc.png" mode=""></image>
					加载状态
				</view>

				<view class="fui-car__content padding-sm margin-xs">
					<view class="flex justify-content align-center padding-tb-sm bg-green">
						<image class="fui-loading-icon loading" src="../../static/images/icons/jzsuccess.png" mode="">
						</image>
						<view class="margin-left-sm">
							加载中...
						</view>
					</view>
				</view>
			</view>
			<!-- 加载状态 end -->

			<!-- 加载错误 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/spdq.png" mode=""></image>
					加载错误
				</view>

				<view class="fui-car__content padding-sm margin-xs">
					<view class="flex justify-content align-center padding-tb-sm bg-red">
						<image class="fui-loading-icon" src="../../static/images/icons/jzerror.png" mode=""></image>
						<view class="margin-left-sm">
							加载失败
						</view>
					</view>
				</view>
			</view>
			<!-- 加载错误 end -->

			<!-- toast start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/dfl.png" mode=""></image>
					toast加载
				</view>

				<view class="fui-car__content padding-sm margin-xs">
					<view class="flex justify-around  align-center padding-tb-sm ">
						<view class=" flex-column justify-content align-center padding-sm  bg-black ">
							<image class="fui-loading-icon loading" src="../../static/images/icons/jzsuccess.png"
								mode="">lable</image>
						</view>
						<view class=" flex justify-content align-center padding-df bg-black ">
							<image class="fui-loading-icon loading" src="../../static/images/icons/jzsuccess.png"
								mode=""></image>
						</view>
					</view>
				</view>
			</view>
			<!-- toast end -->
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
