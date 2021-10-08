<template>
	<view class="">
		<FuiNavBar>
			<block slot="content">头像</block>
		</FuiNavBar>
		<view class="wrap">
			<!-- 头像尺寸形状1 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/czdq.png" mode=""></image>
					头像尺寸形状1
				</view>

				<view class="fui-car__content padding-sm margin-xs">
					<view class="flex align-center">
						<view class="fui-avatar xl round margin-right-xl"
							style="background-image: url(../../static/images/icons/txcxxz1.png);"></view>
						<view class="fui-avatar round margin-right-xl"
							style="background-image: url(../../static/images/icons/txcxxz1.png);"></view>
						<view class="fui-avatar xs round margin-right-xl"
							style="background-image: url(../../static/images/icons/txcxxz1.png);"></view>
						<view class="fui-avatar sm round"
							style="background-image: url(../../static/images/icons/txcxxz1.png);"></view>
					</view>

				</view>
			</view>
			<!-- 头像尺寸形状1 end -->
			<!-- 头像尺寸形状2 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/czdq.png" mode=""></image>
					头像尺寸形状2
				</view>

				<view class="fui-car__content padding-sm margin-xs">
					<view class="flex align-center">
						<view class="fui-avatar xl  margin-right-xl"
							style="background-image: url(../../static/images/icons/txcxxz2.png);"></view>
						<view class="fui-avatar  margin-right-xl"
							style="background-image: url(../../static/images/icons/txcxxz2.png);"></view>
						<view class="fui-avatar xs margin-right-xl"
							style="background-image: url(../../static/images/icons/txcxxz2.png);"></view>
						<view class="fui-avatar sm"
							style="background-image: url(../../static/images/icons/txcxxz2.png);"></view>
					</view>

				</view>
			</view>
			<!-- 头像尺寸形状2 end -->
			<!-- 头像阴影效果 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/czdq.png" mode=""></image>
					头像阴影效果
				</view>

				<view class="fui-car__content padding-sm margin-xs">
					<view class="flex align-center">
						<view class="fui-avatar xl  margin-right-lg shadow"
							style="background-image: url(../../static/images/icons/txcxxz2.png);"></view>
						<view class="fui-avatar  margin-right-lg shadow"
							style="background-image: url(../../static/images/icons/txcxxz2.png);"></view>
						<view class="fui-avatar xl round  margin-right-lg shadow"
							style="background-image: url(../../static/images/icons/txcxxz1.png);"></view>
						<view class="fui-avatar round margin-right-lg shadow"
							style="background-image: url(../../static/images/icons/txcxxz1.png);"></view>
					</view>

				</view>
			</view>
			<!-- 头像阴影效果 end -->
			<!-- 头像内嵌文字/图标 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/czdq.png" mode=""></image>
					头像内嵌文字/图标
				</view>

				<view class="fui-car__content padding-sm margin-xs">
					<view class="flex align-center margin-bottom-sm">
						<view class="fui-avatar round  margin-right-xl"
							style="background-image: url(../../static/images/icons/txnqwz1.png);"></view>
						<view class="fui-avatar round margin-right-xl">陈斌</view>
						<view class="fui-avatar xs round margin-right-xl">陈斌</view>
						<view class="fui-avatar sm round">陈</view>
					</view>
					<view class="flex align-center">
						<view class="fui-avatar radius  margin-right-xl"
							style="background-image: url(../../static/images/icons/jbys.png);"></view>
						<view class="fui-avatar radius margin-right-xl">陈斌</view>
						<view class="fui-avatar xs radius margin-right-xl">陈斌</view>
						<view class="fui-avatar sm radius">陈</view>
					</view>
				</view>
			</view>
			<!-- 头像内嵌文字/图标 end -->
			<!-- 头像带标签 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/czdq.png" mode=""></image>
					头像带标签
				</view>

				<view class="fui-car__content padding-sm margin-xs">
					<view class="flex align-center margin-bottom-sm">
						<view class="fui-badge_wrap margin-right-xl">
							<view class="fui-avatar round  "
								style="background-image: url(../../static/images/icons/txcxxz1.png);"></view>
							<view class="fui-badge fui-tag-xs round bg-red">
								♀
							</view>
						</view>
						<view class="fui-badge_wrap margin-right-xl">
							<view class="fui-avatar round  "
								style="background-image: url(../../static/images/icons/txcxxz2.png);"></view>
							<view class="fui-badge fui-tag-xs round bg-blue">
								♂
							</view>
						</view>
					</view>
				</view>
			</view>
			<!-- 头像带标签 end -->
			<!-- 头像组 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/czdq.png" mode=""></image>
					头像组
				</view>

				<view class="fui-car__content padding-sm margin-xs">
					<view class="flex align-center margin-bottom-sm fui-avatar-group padding-left-sm">
						<view class="fui-avatar round  "
							style="background-image: url(../../static/images/icons/txcxxz1.png);"></view>
						<view class="fui-avatar round  "
							style="background-image: url(../../static/images/icons/txcxxz2.png);"></view>
						<view class="fui-avatar round  "
							style="background-image: url(../../static/images/icons/txcxxz1.png);"></view>
						<view class="fui-avatar round  "
							style="background-image: url(../../static/images/icons/txcxxz2.png);"></view>
						<view class="fui-avatar round  "
							style="background-image: url(../../static/images/icons/txcxxz1.png);"></view>
					</view>
				</view>
			</view>
			<!-- 头像组 end -->
			<!-- 头像组带按钮 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/czdq.png" mode=""></image>
					头像组带按钮
				</view>

				<view class="fui-car__content padding-sm margin-xs">
					<view class="flex align-center margin-bottom-sm fui-avatar-group padding-left-sm">
						<view class="fui-avatar round  " style="background-image: url(../../static/images/icons/txzdan.png);">+</view>
						<view class="fui-avatar round  "
							style="background-image: url(../../static/images/icons/txcxxz1.png);"></view>
						<view class="fui-avatar round  "
							style="background-image: url(../../static/images/icons/txcxxz2.png);"></view>
						<view class="fui-avatar round  "
							style="background-image: url(../../static/images/icons/txcxxz1.png);"></view>
						<view class="fui-avatar round  "
							style="background-image: url(../../static/images/icons/txcxxz2.png);"></view>
						<view class="fui-avatar round  "
							style="background-image: url(../../static/images/icons/txcxxz1.png);"></view>
					</view>
				</view>
			</view>
			<!-- 头像组带按钮 end -->
			<!-- 列表内使用 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/czdq.png" mode=""></image>
					列表内使用
				</view>
			
				<view class="fui-car__content padding-sm margin-xs">
					<view class="flex align-center margin-bottom-sm fui-avatar-group padding-left-sm">
						<view class="fui-avatar xs round  "
							style="background-image: url(../../static/images/icons/txcxxz1.png);"></view>
						<view class="fui-avatar xs round  "
							style="background-image: url(../../static/images/icons/txcxxz2.png);"></view>
						<view class="fui-avatar xs round  "
							style="background-image: url(../../static/images/icons/txcxxz1.png);"></view>
						<view class="fui-avatar xs round  "
							style="background-image: url(../../static/images/icons/txcxxz2.png);"></view>
						<view class="fui-avatar xs round  "
							style="background-image: url(../../static/images/icons/txcxxz1.png);"></view>
					</view>
				</view>
			</view>
			<!-- 列表内使用 end -->
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
