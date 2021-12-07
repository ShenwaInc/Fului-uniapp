<template>
	<view class="">
		<FuiNavBar class="bg-blue">
			<block slot="title">文本</block>
		</FuiNavBar>
		<view class="wrap">
			<!-- 宫格列表 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/czdq.png" mode=""></image>
					宫格列表
				</view>
				<view class="fui-car__content padding-sm margin-xs">
					2列宫格
					<view class="flex line-b padding-tb-sm">
						<view class="col-12 flex align-center justify-around">
							<view style="width: 60rpx;height: 60rpx;" class="bg-red"></view>
							标题文字
						</view>
						<view class="col-12 flex align-center justify-around">
							<view style="width: 60rpx;height: 60rpx;" class="bg-red"></view>
							标题文字
						</view>
					</view>
					3列宫格
					<view class="flex line-b padding-tb-sm">
						<view class="col-8 flex-column align-center justify-around">
							<view style="width: 60rpx;height: 60rpx;" class="bg-red"></view>
							标题文字
						</view>
						<view class="col-8 flex-column align-center justify-around">
							<view style="width: 60rpx;height: 60rpx;" class="bg-red"></view>
							标题文字
						</view>
						<view class="col-8 flex-column align-center justify-around">
							<view style="width: 60rpx;height: 60rpx;" class="bg-red"></view>
							标题文字
						</view>
					</view>
					4列宫格
					<view class="flex line-b padding-tb-sm">
						<view class="col-6 flex-column align-center justify-around">
							<view style="width: 60rpx;height: 60rpx;" class="bg-red"></view>
							标题文字
						</view>
						<view class="col-6 flex-column align-center justify-around">
							<view style="width: 60rpx;height: 60rpx;" class="bg-red"></view>
							标题文字
						</view>
						<view class="col-6 flex-column align-center justify-around">
							<view style="width: 60rpx;height: 60rpx;" class="bg-red"></view>
							标题文字
						</view>
						<view class="col-6 flex-column align-center justify-around">
							<view style="width: 60rpx;height: 60rpx;" class="bg-red"></view>
							标题文字
						</view>
					</view>
					4+N 宫格
					<view class="flex line-b padding-tb-sm">
						<view class="col-5 flex-column align-center justify-around">
							<view style="width: 60rpx;height: 60rpx;" class="bg-red"></view>
							标题
						</view>
						<view class="col-5 flex-column align-center justify-around">
							<view style="width: 60rpx;height: 60rpx;" class="bg-red"></view>
							标题
						</view>
						<view class="col-5 flex-column align-center justify-around">
							<view style="width: 60rpx;height: 60rpx;" class="bg-red"></view>
							标题
						</view>
						<view class="col-5 flex-column align-center justify-around">
							<view style="width: 60rpx;height: 60rpx;" class="bg-red"></view>
							标题
						</view>
						<view class="col-5 flex-column align-center justify-around">
							<view style="width: 60rpx;height: 60rpx;" class="bg-green"></view>
							标题
						</view>
					</view>
					5 宫格
					<view class="flex line-b padding-tb-sm">
						<view class="col-5 flex-column align-center justify-around">
							<view style="width: 60rpx;height: 60rpx;" class="bg-red"></view>
							标题
						</view>
						<view class="col-5 flex-column align-center justify-around">
							<view style="width: 60rpx;height: 60rpx;" class="bg-red"></view>
							标题
						</view>
						<view class="col-5 flex-column align-center justify-around">
							<view style="width: 60rpx;height: 60rpx;" class="bg-red"></view>
							标题
						</view>
						<view class="col-5 flex-column align-center justify-around">
							<view style="width: 60rpx;height: 60rpx;" class="bg-red"></view>
							标题
						</view>
						<view class="col-5 flex-column align-center justify-around">
							<view style="width: 60rpx;height: 60rpx;" class="bg-red"></view>
							标题
						</view>
					</view>
					可滑动宫格
					<view class="flex line-b padding-tb-sm overflow">
						<view class="col-4 flex-column align-center justify-around " v-for="item in 10" :key="item">
							<view style="width: 60rpx;height: 60rpx;" class="bg-red"></view>
							标题
						</view>
					</view>


				</view>
			</view>
			<!-- 宫格列表 end -->
			<!-- 菜单列表 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/czdq.png" mode=""></image>
					菜单列表
				</view>

				<view class="fui-car__content padding-sm margin-xs">
					<view class="fui-cell padding-xs margin-bottom-xs bg-bg_grey">
						<view class="fui-cell__title">
							基础列表
						</view>
						<view class="right-arrow"></view>
					</view>
					<view class="fui-cell padding-xs margin-bottom-xs bg-bg_grey">
						<view class="fui-cell__title">
							提示信息列表
						</view>
						<view class="fui-cell__value">
							详细信息
						</view>
					</view>
					<view class="fui-cell padding-xs margin-bottom-xs bg-bg_grey">
						<view class="fui-cell__title">
							提示+箭头 列表
						</view>
						<view class="fui-cell__value">
							详细信息
						</view>
						<view class="right-arrow"></view>
					</view>
					<view class="fui-cell padding-xs margin-bottom-xs bg-bg_grey">
						<view class="fui-cell__title">
							胶囊按钮列表
						</view>
						<view class="fui-cell__value">
							<uni-button class="fui-button fui-button-df round bg-dodgerblue plain">胶囊按钮</uni-button>
						</view>
					</view>
					<view class="fui-cell padding-xs margin-bottom-xs bg-bg_grey">
						<view class="fui-cell__title">
							开关按钮列表
						</view>
						<view class="fui-cell__value">
							<switch checked="true" />
						</view>
					</view>
					<view class="fui-cell padding-xs margin-bottom-xs bg-bg_grey">
						<view class="fui-cell__title">
							勾选列表
						</view>
						<view class="fui-cell__value">
							√
						</view>
					</view>
					<view class="fui-cell padding-xs margin-bottom-xs bg-bg_grey">
						<view class="">
							？
						</view>
						<view class="fui-cell__title">
							图标+标题列表
						</view>
						<view class="right-arrow"></view>
					</view>
					<view class="fui-cell padding-xs margin-bottom-xs bg-bg_grey">
						<view class="">
							？
						</view>
						<view class="fui-cell__title">
							标签+标题列表
						</view>
						<view class="fui-cell__value flex justify-around">
							<view class="ui-tag  primary light round">
								标签
							</view>
							<view class="ui-tag  error light round">
								标签
							</view>
							<view class="ui-tag  warning light round">
								标签
							</view>
						</view>
					</view>
					
				</view>
			</view>
			<!-- 菜单列表 end -->
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
