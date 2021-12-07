<template>
	<view class="">
		<FuiNavBar class="bg-blue"> 
			<block slot="title">按钮</block>
		</FuiNavBar>
		<view class="wrap">
			<!-- 按钮形状 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/czdq.png" mode=""></image>
					按钮形状
				</view>
			
				<view class="fui-car__content padding-sm margin-xs ">
				<view class="flex justify-between align-center">
					<uni-button class="fui-button fui-button-df">默认按钮</uni-button>
					<uni-button class="fui-button fui-button-df round">胶囊按钮</uni-button>
					<uni-button class="fui-button fui-button-df circle">图</uni-button>
				</view>
				</view>
			</view>
			<!-- 按钮形状 end -->
			<!-- 按钮尺寸 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/czdq.png" mode=""></image>
					按钮尺寸
				</view>
			
				<view class="fui-car__content padding-sm margin-xs ">
				<view class="flex justify-between align-center">
					<uni-button class="fui-button fui-button-xl round">大尺寸</uni-button>
					<uni-button class="fui-button fui-button-df round">默认</uni-button>
					<uni-button class="fui-button fui-button-xs round">小尺寸</uni-button>
				</view>
				</view>
			</view>
			<!-- 按钮尺寸 end -->
			<!-- 按钮阴影 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/czdq.png" mode=""></image>
					按钮阴影
				</view>
			
				<view class="fui-car__content padding-sm margin-xs ">
				<view class="flex justify-between align-center">
					<uni-button class="fui-button fui-button-xl round primary shadow">操作按钮</uni-button>
					<uni-button class="fui-button fui-button-df error shadow">操作按钮</uni-button>
				</view>
				</view>
			</view>
			<!-- 按钮阴影 end -->
			<!-- 按钮颜色 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/spdq.png" mode=""></image>
					按钮颜色
				</view>
				<view class="fui-car__content padding-sm margin-xs ">
				<view class=" flex-wrap justify-between align-center">
					<uni-button class="fui-button fui-button-df bg-plum margin-top-xs">#C239B3</uni-button>
					<uni-button class="fui-button fui-button-df bg-red margin-top-xs">#E0243A</uni-button>
					<uni-button class="fui-button fui-button-df bg-brown margin-top-xs">#B33C24</uni-button>
					<uni-button class="fui-button fui-button-df bg-tawny margin-top-xs">#D67152</uni-button>
					<uni-button class="fui-button fui-button-df bg-green margin-top-xs">#21A366</uni-button>
					<uni-button class="fui-button fui-button-df bg-darkgreen margin-top-xs">#005E50</uni-button>
					<uni-button class="fui-button fui-button-df bg-blue margin-top-xs">#2C5EC2</uni-button>
					<uni-button class="fui-button fui-button-df bg-dodgerblue margin-top-xs">#4F6BED</uni-button>
					<uni-button class="fui-button fui-button-df bg-royalblue margin-top-xs">#004E8C</uni-button>
					<uni-button class="fui-button fui-button-df bg-purple margin-top-xs">#7738B3</uni-button>
					<uni-button class="fui-button fui-button-df bg-maroon margin-top-xs">#750B1C</uni-button>
					<uni-button class="fui-button fui-button-df bg-teal  margin-top-xs">#038387</uni-button>
				</view>
				</view>
			</view>
			<!-- 按钮颜色 end -->
			<!-- 镂空按钮 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/dg.png" mode=""></image>
					镂空按钮
				</view>
				<view class="fui-car__content padding-sm margin-xs ">
				<view class=" flex-wrap justify-between align-center">
					<uni-button class="fui-button fui-button-df bg-plum plain margin-top-xs">#C239B3</uni-button>
					<uni-button class="fui-button fui-button-df bg-red plain margin-top-xs">#E0243A</uni-button>
					<uni-button class="fui-button fui-button-df bg-brown plain margin-top-xs">#B33C24</uni-button>
					<uni-button class="fui-button fui-button-df bg-tawny plain margin-top-xs">#D67152</uni-button>
					<uni-button class="fui-button fui-button-df bg-green plain margin-top-xs">#21A366</uni-button>
					<uni-button class="fui-button fui-button-df bg-darkgreen plain margin-top-xs">#005E50</uni-button>
					<uni-button class="fui-button fui-button-df bg-blue plain margin-top-xs">#2C5EC2</uni-button>
					<uni-button class="fui-button fui-button-df bg-dodgerblue plain margin-top-xs">#4F6BED</uni-button>
					<uni-button class="fui-button fui-button-df bg-royalblue plain margin-top-xs">#004E8C</uni-button>
					<uni-button class="fui-button fui-button-df bg-purple plain margin-top-xs">#7738B3</uni-button>
					<uni-button class="fui-button fui-button-df bg-maroon plain plain margin-top-xs">#750B1C</uni-button>
					<uni-button class="fui-button fui-button-df bg-teal plain  margin-top-xs">#038387</uni-button>
				</view>
				</view>
			</view>
			<!-- 镂空按钮 end -->
			<!-- 置底按钮 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/gdcc.png" mode=""></image>
					置底按钮
				</view>
				<view class="fui-car__content padding-sm margin-xs bg-bg_grey">
				<view class=" flex-column  font-xl  ">
					<view class="margin-tb-sm">
						置底单按钮
					</view>
					<view class="padding-tb-xs bg-white">
						<uni-button class="fui-button fui-button-xl primary   font-xl">页面主要操作</uni-button>
					</view>
				</view>
				<view class=" flex-column  font-xl  ">
					<view class="margin-tb-sm">
						置底单按钮
					</view>
					<view class="flex padding-tb-xs bg-white">
						<uni-button class="fui-button fui-one margin-right-xs fui-button-xl primary light  font-xl">辅助操作</uni-button>
						<uni-button class="fui-button fui-one fui-button-xl primary   font-xl">主要操作</uni-button>
					</view>
				</view>
				<view class=" flex-column  font-xl  ">
					<view class="margin-tb-sm ">
						置底按钮带icon
					</view>
					<view class="flex padding-tb-xs bg-white align-center">
						<view class="flex-column align-center margin-right-sm">
							<uni-button class="fui-button fui-button-df circle">图</uni-button>
							<view class="font-sm text-grey">
								辅助操作
							</view>
						</view>
						<uni-button class="fui-button fui-one fui-button-xl primary   font-xl">主要操作</uni-button>
					</view>
				</view>
				<view class=" flex-column  font-xl  ">
					<view class="margin-tb-sm ">
						置底按钮带2 icon
					</view>
					<view class="flex padding-tb-xs bg-white align-center">
						<view class="flex-column align-center margin-right-sm">
							<uni-button class="fui-button fui-button-df circle">图</uni-button>
							<view class="font-sm text-grey">
								辅助操作
							</view>
						</view>
						<view class="flex-column align-center margin-right-sm">
							<uni-button class="fui-button fui-button-df circle">图</uni-button>
							<view class="font-sm text-grey">
								辅助操作
							</view>
						</view>
						<uni-button class="fui-button fui-one fui-button-xl primary   font-xl">主要操作</uni-button>
					</view>
				</view>
				<view class=" flex-column  font-xl  ">
					<view class="margin-tb-sm ">
						置底按钮带3 icon
					</view>
					<view class="flex padding-tb-xs bg-white align-center">
						<view class="flex-column align-center margin-right-sm">
							<uni-button class="fui-button fui-button-df circle">图</uni-button>
							<view class="font-sm text-grey">
								辅助操作
							</view>
						</view>
						<view class="flex-column align-center margin-right-sm">
							<uni-button class="fui-button fui-button-df circle">图</uni-button>
							<view class="font-sm text-grey">
								辅助操作
							</view>
						</view>
						<view class="flex-column align-center margin-right-sm">
							<uni-button class="fui-button fui-button-df circle">图</uni-button>
							<view class="font-sm text-grey">
								辅助操作
							</view>
						</view>
						<uni-button class="fui-button fui-one fui-button-xl primary   font-xl">主要操作</uni-button>
					</view>
				</view>
				<view class=" flex-column  font-xl  ">
					<view class="margin-tb-sm">
						主按钮辅助操作
					</view>
					<view class="padding-tb-xs ">
						<uni-button class="fui-button fui-button-xl   bg-white font-xl">辅助操作</uni-button>
					</view>
				</view>
				<view class=" flex-column  font-xl  ">
					<view class="margin-tb-sm">
						主按钮不可操作
					</view>
					<view class="padding-tb-xs ">
						<uni-button Disable class="fui-button fui-button-xl   bg-white font-xl">辅助操作 Disable</uni-button>
					</view>
				</view>
				<view class=" flex-column  font-xl  ">
					<view class="margin-tb-sm">
						警告
					</view>
					<view class="padding-tb-xs ">
						<uni-button  class="fui-button fui-button-xl error  bg-white font-xl">警告类操作</uni-button>
					</view>
				</view>
				</view>
			</view>
			<!-- 置底按钮 end -->
		</view>
	</view>
</template>

<script>
	import FuiNavBar from '@/common/FuiNavBar.vue'
	export default{
		components:{FuiNavBar}
	}
</script>

<style>
</style>
