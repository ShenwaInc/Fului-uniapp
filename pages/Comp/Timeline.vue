<template>
	<view class="">
		<FuiNavBar class="bg-blue"> 
			<block slot="title">时间轴</block>
		</FuiNavBar>
		<view class="wrap">
			<!-- 时间轴1 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/czdq.png" mode=""></image>
					时间轴1
				</view>
				<view class="fui-car__content padding-sm margin-xs">
				<view class="fui-timeline">
					<view class="fui-timeline__item ">
						<image class="fui-timeline__icon" src="../../static/images/icons/shijianxian.png" mode=""></image>
						<view class="fui-timeline__content primary ">
							当你需要一根针时，千万不要去磨铁棒
						</view>
					</view>
					<view class="fui-timeline__item ">
						<image class="fui-timeline__icon" src="../../static/images/icons/shijainxian1.png" mode=""></image>
						<view class="fui-timeline__content error">
							与其等待与能力匹配的机会，不如培养与机会匹配的能力
						</view>
						
					</view>
					<view class="fui-timeline__item ">
						<image class="fui-timeline__icon" src="../../static/images/icons/shijianxian.png" mode=""></image>
						<view class="fui-timeline__content warning">
							与其怕失败，不如狠狠地失败一次
						</view>
						
					</view>
				</view>
				</view>
			</view>
			<!-- 时间轴1 end -->
			<!-- 时间轴2 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/czdq.png" mode=""></image>
					时间轴2
				</view>
				<view class="fui-car__content padding-sm margin-xs">
				<view class="fui-timeline">
					<view class="fui-timeline__item dashed">
						<image class="fui-timeline__icon xl" src="../../static/images/icons/shijianxian2.png" mode=""></image>
						<view class="fui-timeline__content  ">
							<view class="font-df">
								状态显示
							</view>
							<view class="font-lg text-grey">
								灵感是业余者的专属，我们专业人士只要在早上打卡上班即可
							</view>
						</view>
					</view>
					<view class="fui-timeline__item dashed">
						<image class="fui-timeline__icon xl" src="../../static/images/icons/shijianxian2.png" mode=""></image>
						<view class="fui-timeline__content ">
							<view class="font-df">
								状态显示
							</view>
							<view class="font-lg text-grey">
								灵感是业余者的专属，我们专业人士只要在早上打卡上班即可
							</view>
						</view>
						
					</view>
					<view class="fui-timeline__item dashed">
						<image class="fui-timeline__icon xl" src="../../static/images/icons/shijianxian2.png" mode=""></image>
						<view class="fui-timeline__content ">
							<view class="font-df">
								状态显示
							</view>
							<view class="font-lg text-grey">
								灵感是业余者的专属，我们专业人士只要在早上打卡上班即可
							</view>
						</view>
						
					</view>
					<view class="fui-timeline__item dashed">
						<image class="fui-timeline__icon xl" src="../../static/images/icons/shijianxian2.png" mode=""></image>
						<view class="fui-timeline__content ">
							<view class="font-df">
								状态显示
							</view>
							<view class="font-lg text-grey">
								灵感是业余者的专属，我们专业人士只要在早上打卡上班即可
							</view>
						</view>
						
					</view>
				</view>
				</view>
			</view>
			<!-- 时间轴2 end -->
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
