<template>
	<view class="">
		<FuiNavBar>
			<block slot="content">文本</block>
		</FuiNavBar>
		<view class="wrap">
			<!-- 图标 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/czdq.png" mode=""></image>
					图标
				</view>
			
				<view class="fui-car__content padding-sm margin-xs">
				空
					
				</view>
			</view>
			<!-- 图标 end -->
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
