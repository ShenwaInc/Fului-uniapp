<template>
	<view class="">
		<FuiNavBar>
			<block slot="content">进度条</block>
		</FuiNavBar>
		<view class="wrap">
			<!-- 线形进度条 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/czdq.png" mode=""></image>
					线形进度条
				</view>

				<view class="fui-car__content padding-sm margin-xs">
					<view class="fui-process xs round margin-bottom-lg">
						<view :style="{width:width +'%'}" class="fui-process--inner bg-green round"></view>
					</view>
					<view class="fui-process--wrap">
						<view class="fui-process xs round">
							<view :style="{width:width +'%'}" class="fui-process--inner bg-blue round"></view>
						</view>
						<view class="fui-process--text">
							<image style="width: 40rpx;height: 40rpx;" src="../../static/images/icons/jdt.png" mode="">
							</image>
						</view>
					</view>

				</view>
			</view>
			<!-- 线形进度条 end -->
			<!-- 百分比内显进度条 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/czdq.png" mode=""></image>
					百分比内显进度条
				</view>

				<view class="fui-car__content padding-sm margin-xs">
					<view class="fui-process  round margin-bottom-lg">
						<view :style="{width:width +'%'}" class="fui-process--inner bg-blue round">{{width}}%</view>
					</view>
					<view class="fui-process  round ">
						<view :style="{width:width +'%'}" class="fui-process--inner bg-green round">{{width}}%</view>
					</view>
				</view>
			</view>
			<!-- 百分比内显进度条 end -->
			<!-- 条纹进度条 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/czdq.png" mode=""></image>
					条纹进度条
				</view>

				<view class="fui-car__content padding-sm margin-xs">
					<view class="fui-process--wrap">
						<view class="fui-process streak  round">
							<view :style="{width:width +'%'}" class="fui-process--inner bg-blue round"></view>
						</view>
						<view class="fui-process--text">
							{{width}}%
						</view>
					</view>
				</view>
			</view>
			<!-- 条纹进度条 end -->
			<!-- 条纹进度条 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/czdq.png" mode=""></image>
					条纹进度条
				</view>
				<view class="fui-car__content padding-sm margin-xs">
					<view class="fui-process streak round ">
						<view :style="{width:width +'%'}" class="fui-process--inner bg-red ">30%</view>
						<view :style="{width:width +'%'}" class="fui-process--inner bg-blue ">45%</view>
						<view :style="{width:width +'%'}" class="fui-process--inner bg-green ">25%</view>
					</view>
				</view>
			</view>
			<!-- 条纹进度条 end -->
			<!-- 环形进度条 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/czdq.png" mode=""></image>
					环形进度条
				</view>
				<view class="fui-car__content padding-sm margin-xs">
					<view class="flex justify-between">
						<view class="fui-process--circle">
							<svg viewBox="0 0 100 100">
								<path d="M 50 50 m 0 -47 a 47 47 0 1 1 0 94 a 47 47 0 1 1 0 -94" stroke="#e5e9f2"
									stroke-width="4.8" fill="none"></path>
								<path d="M 50 50 m 0 -47 a 47 47 0 1 1 0 94 a 47 47 0 1 1 0 -94" stroke-linecap="round"
									stroke="#2C5EC2" stroke-width="4.8" fill="none"
									:style="{strokeDasharray:299.08+width*2.92+'px'}"
									style="stroke-dashoffset: 299.08px;">
								</path>
							</svg>
							<view class="fui-process--text">
								{{width}}%
							</view>
						</view>

						<view class="fui-process--circle">
							<svg viewBox="0 0 100 100">
								<path d="M 50 50 m 0 -47 a 47 47 0 1 1 0 94 a 47 47 0 1 1 0 -94" stroke="#e5e9f2"
									stroke-width="4.8" fill="none"></path>
								<path d="M 50 50 m 0 -47 a 47 47 0 1 1 0 94 a 47 47 0 1 1 0 -94" stroke-linecap="round"
									stroke="#E8484C" stroke-width="4.8" fill="none"
									:style="{strokeDasharray:299.08+width*2.92+'px'}"
									style="stroke-dashoffset: 299.08px;">
								</path>
							</svg>
							<view class="fui-process--text">
								{{width}}%
							</view>
						</view>

						<view  class="fui-process--circle">
							<svg viewBox="0 0 100 100">
								<path d="M 50 50 m 0 -47 a 47 47 0 1 1 0 94 a 47 47 0 1 1 0 -94" stroke="#e5e9f2"
									stroke-width="4.8" fill="none"></path>
								<path d="M 50 50 m 0 -47 a 47 47 0 1 1 0 94 a 47 47 0 1 1 0 -94" stroke-linecap="round"
									stroke="#1B8841" stroke-width="4.8" fill="none"
									:style="{strokeDasharray:299.08+width*2.92+'px'}"
									style="stroke-dashoffset: 299.08px;">
								
								</path>
							</svg>
							<view class="fui-process--text font-xxl" style="color: #1B8841;">
								√
							</view>
						</view>
					</view>
				</view>
			</view>
			<!-- 环形进度条 end -->
		</view>
	</view>
</template>

<script>
	import FuiNavBar from '@/common/FuiNavBar.vue'
	export default {
		components: {
			FuiNavBar
		},
		data(){
			return{
				// :style="{stroke-dashoffset: 299.08+width*2.92+'px';}"
				width:0
			}
		},
		mounted(){
			setInterval(()=>{
				if(this.width<100){
					this.width++
				}
			},1000/60)
		}
	}
</script>

<style>
</style>
