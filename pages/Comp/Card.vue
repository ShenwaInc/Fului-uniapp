<template>
	<view class="">
		<FuiNavBar class="bg-blue">
			<block slot="title">文本</block>
		</FuiNavBar>
		<view class="wrap">
			<!-- 案例类卡片 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/czdq.png" mode=""></image>
					案例类卡片
				</view>
				<view class="fui-car__content ">
					<image style="width: 100%" src="../../static/images/icons/card1.png" mode=""></image>
				</view>
				<view class="fui-car__foot flex padding-sm margin-xs">
					<image class="fui-avatar xl round" src="../../static/images/icons/txcxxz2.png" mode=""></image>
					<view class="flex-column justify-around margin-left-xl">
						<text>Adelaide Ramos</text>
						<text class="font-xs text-grey">24天前</text>
					</view>
				</view>
			</view>
			<!-- 案例类卡片 end -->
			<!-- 动态类卡片 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/czdq.png" mode=""></image>
					动态类卡片
				</view>
				<view class="fui-car__header padding-sm margin-xs">
					<image class="fui-avatar xl round" src="../../static/images/icons/txcxxz2.png" mode=""></image>
					<view class="flex-column justify-around margin-left-xl">
						<text>Adelaide Ramos</text>
						<text class="font-xs text-grey">2021年09月22日</text>
					</view>

				</view>
				<view class="fui-car__content line-b">
					<view class="padding-lr-sm margin-xs">
						梦想不足以让你到达远方，但是到达远方的人一定要有梦想
					</view>
					<image class="padding-lr-df" style="width: 100%" src="../../static/images/icons/card1.png" mode="">
					</image>
					<view class="padding-lr-df flex justify-end text-grey padding-tb-df">
						<view class="margin-right-df ">
							<image style="width: 15px;height: 15px;" src="../../static/images/icons/liulan.png" mode="">
							</image>
							67
						</view>
						<view class="margin-right-df">
							<image style="width: 15px;height: 15px;" src="../../static/images/icons/dianzan.png"
								mode=""></image>
							25
						</view>
						<view class="">
							<image style="width: 15px;height: 15px;" src="../../static/images/icons/pinglun.png"
								mode=""></image>
							32
						</view>
					</view>
				</view>
				<view class="fui-car__foot flex-column padding-sm margin-xs">
					<view class="flex margin-bottom-df">
						<image class="fui-avatar xs round margin-right-df" src="../../static/images/icons/txcxxz1.png"
							mode=""></image>
						<view class="flex-column line-b fui-one">
							<view class="">
								Derek Gibson
							</view>
							<view class="">
								说了不一定有机会，但不说一定没机会
							</view>
							<view class="text-grey flex justify-between font-xs">
								<view class="">
									2021年09月22日
								</view>
								<view class="">
									<image class="margin-right-df" style="width: 15px;height: 15px;"
										src="../../static/images/icons/dianzan.png" mode=""></image>
									<image style="width: 15px;height: 15px;" src="../../static/images/icons/pinglun.png"
										mode=""></image>
								</view>
							</view>
						</view>
					</view>
					<view class="flex">
						<image class="fui-avatar xs round margin-right-df" src="../../static/images/icons/txcxxz2.png"
							mode=""></image>
						<view class="flex-column line-b fui-one">
							<view class="">
								Caroline Tucker
							</view>
							<view class="">
								改变别人之前，先改变自己
							</view>
							<view class="text-grey flex justify-between font-xs">
								<view class="">
									2021年09月22日
								</view>
								<view class="">
									<image class="margin-right-df" style="width: 15px;height: 15px;"
										src="../../static/images/icons/dianzan.png" mode=""></image>
									<image style="width: 15px;height: 15px;" src="../../static/images/icons/pinglun.png"
										mode=""></image>
								</view>
							</view>
						</view>
					</view>
				</view>
			</view>
			<!-- 动态类卡片 end -->
			<!-- 文章类卡片 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/czdq.png" mode=""></image>
					文章类卡片
				</view>
				<view class="fui-car__header padding-sm margin-xs font-xl bold">
					不要给失败找理由，要为成功找方向
				</view>
				<view class="fui-car__content padding-lr-df padding-bottom-df">
					<view class="flex">
						<image style="width: 120px;height: 90px;" src="../../static/images/icons/card1.png" mode="">
						</image>
						<view class="fui-one padding-left-df">
							<view class="text-grey font-lg">
								在项目伊始时做一个用户研究的作用好过于在项目落地后再对50个用户进行测试…
							</view>
							<view class="flex margin-top-xs">
								<view class="fui-tag primary light round">
									标签
								</view>
								<view class="fui-tag error light round">
									标签
								</view>
								<view class="fui-tag warning light round">
									标签
								</view>
							</view>
						</view>
					</view>
				</view>

			</view>
			<!-- 文章类卡片 end -->
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
