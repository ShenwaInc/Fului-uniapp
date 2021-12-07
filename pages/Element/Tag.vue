<template>
	<view class="">
		<FuiNavBar class="bg-blue"> 
			<block slot="title">文本</block>
		</FuiNavBar>
		<view class="wrap">
			<!-- 标签形状 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/czdq.png" mode=""></image>
					标签形状
				</view>
				<view class="fui-car__content padding-sm margin-xs">
					<view class="flex justify-between align-center">
						<view class="fui-tag">默认</view>
						<view class="fui-tag radius">圆角</view>
						<view class="fui-tag round">胶囊</view>
						<view class="fui-tag circle">12</view>
					</view>
				</view>
			</view>
			<!-- 标签形状 end -->
			<!-- 标签尺寸 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/czdq.png" mode=""></image>
					标签尺寸
				</view>
				<view class="fui-car__content padding-sm margin-xs">
					<view class="flex justify-between align-center">
						<view class="fui-tag">默认尺寸</view>
						<view class="fui-tag-xs ">小尺寸</view>

					</view>
				</view>
			</view>
			<!-- 标签尺寸 end -->
			<!-- 标签阴影 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/czdq.png" mode=""></image>
					标签阴影
				</view>
				<view class="fui-car__content padding-sm margin-xs">
					<view class="flex justify-between">
						<view class="fui-tag round primary shadow">胶囊</view>
						<view class="fui-tag error shadow">默认</view>
					</view>
				</view>
			</view>
			<!-- 标签阴影 end -->
			<!-- 标签颜色 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/dg.png" mode=""></image>
					标签颜色
				</view>
				<view class="fui-car__content padding-lr-sm margin-xs">
					重色填充
				</view>
				<view class="fui-car__content padding-sm margin-xs ">
					<view class=" flex-wrap justify-between align-center">
						<view class="fui-tag bg-plum  margin-top-xs">#C239B3</view>
						<view class="fui-tag bg-red  margin-top-xs">#E0243A</view>
						<view class="fui-tag bg-brown  margin-top-xs">#B33C24</view>
						<view class="fui-tag bg-tawny  margin-top-xs">#D67152</view>
						<view class="fui-tag bg-green  margin-top-xs">#21A366</view>
						<view class="fui-tag bg-darkgreen  margin-top-xs">#005E50</view>
						<view class="fui-tag bg-blue  margin-top-xs">#2C5EC2</view>
						<view class="fui-tag bg-dodgerblue  margin-top-xs">#4F6BED</view>
						<view class="fui-tag bg-royalblue  margin-top-xs">#004E8C</view>
						<view class="fui-tag bg-purple  margin-top-xs">#7738B3</view>
						<view class="fui-tag bg-maroon  margin-top-xs">#750B1C</view>
						<view class="fui-tag bg-teal   margin-top-xs">#038387</view>
					</view>
				</view>
				<view class="fui-car__content padding-lr-sm margin-xs">
					浅色填充
				</view>
				<view class="fui-car__content padding-sm margin-xs ">
					<view class=" flex-wrap justify-between align-center">
						<view class="fui-tag  primary light margin-top-xs">#CCE6FF</view>
						<view class="fui-tag  error light margin-top-xs">#FFF3F4</view>
						<view class="fui-tag  warning light margin-top-xs">#E2DDCC</view>
					</view>
				</view>
			</view>
			<!-- 标签颜色 end -->
			<!-- 镂空标签 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/dg.png" mode=""></image>
					镂空标签
				</view>
				<view class="fui-car__content padding-sm margin-xs ">
					<view class=" flex-wrap justify-between align-center">
						<view class="fui-tag bg-plum plain margin-top-xs">#C239B3</view>
						<view class="fui-tag bg-red plain margin-top-xs">#E0243A</view>
						<view class="fui-tag bg-brown plain margin-top-xs">#B33C24</view>
						<view class="fui-tag bg-tawny plain margin-top-xs">#D67152</view>
						<view class="fui-tag bg-green plain margin-top-xs">#21A366</view>
						<view class="fui-tag bg-darkgreen plain margin-top-xs">#005E50</view>
						<view class="fui-tag bg-blue plain margin-top-xs">#2C5EC2</view>
						<view class="fui-tag bg-dodgerblue plain margin-top-xs">#4F6BED</view>
						<view class="fui-tag bg-royalblue plain margin-top-xs">#004E8C</view>
						<view class="fui-tag bg-purple plain margin-top-xs">#7738B3</view>
						<view class="fui-tag bg-maroon plain plain margin-top-xs">#750B1C</view>
						<view class="fui-tag bg-teal plain  margin-top-xs">#038387</view>
					</view>
				</view>
			</view>
			<!-- 镂空标签 end -->
		
			<!-- 角标样式 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/czdq.png" mode=""></image>
					角标样式
				</view>
				<view class="fui-car__content padding-sm margin-xs">
					<view class="flex  justify-between align-center">
						<view class="fui-badge_wrap ">
							 	<image style="width: 120rpx;height: 120rpx;" src="../../static/images/icons/jbys.png" mode=""></image>
							<view class="fui-badge fui-tag-xs round primary">
								99+
							</view>
						</view>
						<view class="fui-badge_wrap ">
							 	<image style="width: 120rpx;height: 120rpx;" src="../../static/images/icons/jbys.png" mode=""></image>
							<view class="fui-badge  fui-tag-xs round primary">
								6
							</view>
						</view>
						<view class="fui-badge_wrap ">
							 	<image style="width: 120rpx;height: 120rpx;" src="../../static/images/icons/jbys.png" mode=""></image>
							<view class="fui-badge fui-badge--dot fui-tag-xs  primary">
								
							</view>
						</view>
						<view class="fui-badge_wrap ">
							 	<image style="width: 120rpx;height: 120rpx;" src="../../static/images/icons/jbys.png" mode=""></image>
							<view class="fui-badge fui-tag-xs fui-badge--tag  primary">
								文字
							</view>
						</view>
						
					</view>
				</view>
			</view>
			<!-- 角标样式 end -->
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
