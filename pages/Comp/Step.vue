<template>
	<view class="">
		<FuiNavBar class="bg-blue">
			<block slot="title">步骤条</block>
		</FuiNavBar>
		<view class="wrap">
			<!-- 数字步骤条 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/czdq.png" mode=""></image>
					数字步骤条
				</view>

				<view class="fui-car__content padding-sm margin-xs">
					<view class="fui-steps">
						<view class="fui-steps__item" :class="item>num?'':'finish'" v-for="item in 4" :key="item">
							<view class="fui-steps__title">{{item}}</view> 进度
						</view>
					</view>
				</view>
			</view>
			<!-- 数字步骤条 end -->
			<!-- 图标步骤条 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/czdq.png" mode=""></image>
					图标步骤条
				</view>

				<view class="fui-car__content padding-sm margin-xs">
					<view class="fui-steps">
						<view class="fui-steps__item" :class="item>num?'':'finish'" v-for="item in 4" :key="item">
							<view class="fui-steps__title">?</view> 进度
						</view>
					</view>
				</view>
			</view>
			<!-- 图标步骤条 end -->
			<!-- 箭头分隔步骤条 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/czdq.png" mode=""></image>
					箭头分隔步骤条
				</view>

				<view class="fui-car__content padding-sm margin-xs">
					<view class="fui-steps arrow">
						<view class="fui-steps__item" :class="item>num?'':'finish'" v-for="item in 4" :key="item">
							<view class="fui-steps__title">?</view> 进度
						</view>
					</view>
				</view>
			</view>
			<!-- 箭头分隔步骤条 end -->
			<!-- 圆点步骤条 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/czdq.png" mode=""></image>
					圆点步骤条
				</view>
				<view class="fui-car__content padding-sm margin-xs">
					<view class="fui-steps__dot ">
						<view class="fui-steps__item" :class="item>num?'':'finish'" v-for="item in 4" :key="item">
							<view class="fui-steps__title"></view>
							<text class="font-sm padding-top-sm">标题</text>
							<text class="font-xs  padding-top-sm">小标</text>
						</view>
					</view>
				</view>
			</view>
			<!-- 圆点步骤条 end -->
			
		</view>
	</view>
</template>

<script>
	import FuiNavBar from '@/common/FuiNavBar.vue'
	export default {
		components: {
			FuiNavBar
		},
		data() {
			return {
				num: 0
			}
		},
		onLoad() {
			setInterval(() => {
				if (this.num < 4) {
					this.num++
				} else {
					this.num = 0
				}

			}, 1000)
		}
	}
</script>

<style>
	
</style>
