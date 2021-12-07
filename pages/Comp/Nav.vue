<template>
	<view class="">
		<FuiNavBar class="bg-blue"> 
			<block slot="title">选项卡</block>
		</FuiNavBar>
		<view class="wrap">
			<!-- 平分 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/czdq.png" mode=""></image>
					平分
				</view>
				<view class="fui-car__content ">
					<scroll-view scroll-x >
						<view class="flex">
							<view  class="fui-tab" :class="{'fui-tab--active':active ==index}" v-for="(item,index) in 3" :key='index' @tap="clickTab(index)">{{`Tab${index}`}}</view>
						</view>
					</scroll-view>
				</view>
			</view>
			<!-- 平分 end -->
			<!-- 居中 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/czdq.png" mode=""></image>
					居中
				</view>
				<view class="fui-car__content ">
					<scroll-view scroll-x class="text-cente">			
							<view  class="fui-tab" :class="{'fui-tab--active':active ==index}" v-for="(item,index) in 3" :key='index' @tap="clickTab(index)">{{`Tab${index}`}}</view>
					</scroll-view>
				</view>
			</view>
			<!-- 居中 end -->
			<!-- 背景 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/czdq.png" mode=""></image>
					背景
				</view>
				<view class="fui-car__content ">
					<scroll-view scroll-x class="text-cente bg-red">			
							<view  class="fui-tab" :class="{'fui-tab--active':active ==index}" v-for="(item,index) in 3" :key='index' @tap="clickTab(index)">{{`Tab${index}`}}</view>
					</scroll-view>
				</view>
			</view>
			<!-- 背景 end -->
			<!-- 图标 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/czdq.png" mode=""></image>
					图标
				</view>
				<view class="fui-car__content ">
					<scroll-view scroll-x class="text-cente bg-red">			
							<view  class="fui-tab" :class="{'fui-tab--active':active ==index}" v-for="(item,index) in 3" :key='index' @tap="clickTab(index)">
								<image style="width: 30rpx;height: 30rpx;" src="../../static/images/icons/tab0.png" mode=""></image>
							{{`Tab${index}`}}</view>
					</scroll-view>
				</view>
			</view>
			<!-- 图标 end -->
		</view>
	</view>
</template>

<script>
	import FuiNavBar from '@/common/FuiNavBar.vue'
	export default{
		components:{FuiNavBar},
		data(){
			return{
				active:0
			}
		},methods:{
			clickTab(index){
				this.active=index
				
			}
		}
	}
</script>

<style>
</style>
