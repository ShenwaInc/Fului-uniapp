<template>
	<view class="">
		<FuiNavBar class="bg-blue">
			<block slot="title">意见反馈</block>
		</FuiNavBar>
		<view class="wrap">
			<!-- 问题描述 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/czdq.png" mode=""></image>
					问题描述
				</view>

				<view class="fui-car__content padding-sm margin-xs">
					<textarea value="" class="bg-bg_light_gray" placeholder="请填写十个字以上的问题描述以便我们提供更好的帮助和改进" />

				</view>
			</view>
			<!-- 问题描述 end -->
			<!-- 相关截图(选填） start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/czdq.png" mode=""></image>
					相关截图(选填）
				</view>

				<view class="fui-car__content padding-sm margin-xs">
					<view class="flex justify-around">
						<view class="fui-uploader" @tap="Upload">

							<view class="fui-uploader__wrapper">
								<view class="fui-uploader__upload bg-darkgrey ">
									<text class="font-df ">上传成功</text>
									<icon class="fui-uploader__clear" type="clear" size="17" color="#E94F4F" />
								</view>
							</view>
						</view>
						<view class="fui-uploader" @tap="Upload">
							<view class="fui-uploader__wrapper">
								<view class="fui-uploader__upload bg-bg_grey">
									<icon type="waiting" size="26" />
								</view>
							</view>
						</view>
					</view>

				</view>
			</view>
			<!-- 相关截图(选填） end -->
			<!-- 联系方式 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/czdq.png" mode=""></image>
					联系方式
				</view>

				<view class="fui-car__content padding-sm margin-xs">
					<view class="  fui-form solid">
						<input type="text" placeholder="请填写邮箱/手机号" />
					</view>

				</view>
			</view>
			<!-- 联系方式 -->


		</view>
		<view style="position: fixed;
    bottom: 0;
    left: 0;
    right: 0;">
			<uni-button class="fui-button fui-button-xl primary   font-xl">提交</uni-button>
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
