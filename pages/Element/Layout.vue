<template>
	<view class="">
		<FuiNavBar>
			<block slot="content">布局</block>
		</FuiNavBar>
		<view class="wrap">
			<view class="wrap-item margin-top-xl  fui-tabs shadow radius">
				<view @tap="onTopTab(1)" class="fui-tab" :class="{'fui-tab--active':TabIndex==1}">
					Flex布局
				</view>
				<view @tap="onTopTab(2)" class="fui-tab" :class="{'fui-tab--active':TabIndex==2}">
					Grid布局
				</view>
				<view @tap="onTopTab(3)" class="fui-tab" :class="{'fui-tab--active':TabIndex==3}">
					辅助布局
				</view>
			</view>

			<view v-show="TabIndex==1">
				<!-- 固定尺寸 start -->
				<view class="fui-car wrap-item margin-top-xl  shadow radius">
					<view class="fui-car__header padding-sm margin-xs">
						<image src="../../static/images/icons/gdcc.png" mode=""></image>
						固定尺寸
					</view>
					<view class="fui-car__content padding-sm ">
						<view class="flex flex-wrap">
							<view class="fui-xs bg-green margin-xs padding-sm">
								xs(20%)
							</view>
							<view class="fui-df margin-xs padding-sm">

							</view>
							<view class="fui-sm bg-green  margin-xs padding-sm">
								sm(40%)
							</view>
							<view class="fui-df margin-xs padding-sm">

							</view>
							<view class="fui-df margin-xs bg-green padding-sm">
								df(50%)
							</view>
							<view class="fui-lg bg-green margin-xs padding-sm">
								lg(60%)
							</view>
							<view class="fui-xl bg-green margin-xs padding-sm">
								xl(80%)
							</view>
						</view>
					</view>
				</view>
				<!-- 固定尺寸 end -->
				<!-- 比例布局 start -->
				<view class="fui-car wrap-item margin-top-xl  shadow radius">
					<view class="fui-car__header padding-sm margin-xs">
						<image src="../../static/images/icons/blbj.png" mode=""></image>
						比例布局
					</view>
					<view class="fui-car__content padding-sm ">
						<view class="flex flex-column">
							<view class="flex fui-one">
								<view class="fui-one bg-purple margin-xs padding-sm">
									1
								</view>
								<view class="fui-one bg-purple margin-xs padding-sm">
									1
								</view>
							</view>
							<view class="flex fui-one">
								<view class="fui-one bg-purple margin-xs padding-sm">
									1
								</view>
								<view class="fui-two bg-purple margin-xs padding-sm">
									2
								</view>
							</view>
							<view class="flex fui-one">
								<view class="fui-one bg-purple margin-xs padding-sm">
									1
								</view>
								<view class="fui-two bg-purple margin-xs padding-sm">
									2
								</view>
								<view class="fui-three bg-purple margin-xs padding-sm">
									3
								</view>
							</view>
						</view>
					</view>
				</view>
				<!-- 比例布局end -->
				<!-- 水平对齐 start -->
				<view class="fui-car wrap-item margin-top-xl  shadow radius">
					<view class="fui-car__header padding-sm margin-xs">
						<image src="../../static/images/icons/spdq.png" mode=""></image>
						水平对齐
					</view>
					<view class="fui-car__content padding-sm ">
						<view class="flex flex-column">
							<view class="flex justify-content line-b">
								<view class="bg-red margin-xs padding-sm">
									content
								</view>
								<view class="bg-red margin-xs padding-sm">
									content
								</view>
							</view>
							<view class="flex justify-start line-b">
								<view class="bg-red margin-xs padding-sm">
									start
								</view>
								<view class="bg-red margin-xs padding-sm">
									start
								</view>
							</view>
							<view class="flex justify-end  line-b">
								<view class="bg-red margin-xs padding-sm">
									end
								</view>
								<view class="bg-red margin-xs padding-sm">
									end
								</view>
							</view>
							<view class="flex justify-between line-b ">
								<view class="bg-red margin-xs padding-sm">
									between
								</view>
								<view class="bg-red margin-xs padding-sm">
									between
								</view>
							</view>
							<view class="flex justify-around line-b ">
								<view class="bg-red margin-xs padding-sm">
									around
								</view>
								<view class="bg-red margin-xs padding-sm">
									around
								</view>
							</view>
							<view class="flex justify-evenly  ">
								<view class="bg-red margin-xs padding-sm">
									evenly
								</view>
								<view class="bg-red margin-xs padding-sm">
									evenly
								</view>
							</view>
						</view>
					</view>
				</view>
				<!-- 水平对齐 end -->
				<!-- 垂直对齐 start -->
				<view class="fui-car wrap-item margin-top-xl  shadow radius">
					<view class="fui-car__header padding-sm margin-xs">
						<image src="../../static/images/icons/czdq.png" mode=""></image>
						垂直对齐
					</view>
					<view class="fui-car__content padding-sm ">
						<view class="flex flex-column">
							<view class="flex align-center  line-b">
								<view class="bg-blue margin-xs padding-lg">
									Layout
								</view>
								<view class="bg-blue margin-xs padding-sm">
									content
								</view>
							</view>
							<view class="flex align-start line-b">
								<view class="bg-blue margin-xs padding-lg">
									Layout
								</view>
								<view class="bg-blue margin-xs padding-sm">
									start
								</view>
							</view>
							<view class="flex align-end line-b">
								<view class="bg-blue margin-xs padding-lg">
									Layout
								</view>
								<view class="bg-blue margin-xs padding-sm">
									end
								</view>
							</view>
						</view>
					</view>
				</view>
				<!-- 垂直对齐 end-->
			</view>
			<view v-show="TabIndex==2">
				<!-- 等分列 start-->
				<view class="fui-car wrap-item margin-top-xl  shadow radius">
					<view class="fui-car__header padding-sm margin-xs">
						<image src="../../static/images/icons/dfl.png" mode=""></image>
						等分列
					</view>
					<view class="fui-car__content padding-sm ">
						<view class="row margin-xs">
							<view class="col-24 bg-brown padding-sm">
								24
							</view>
							<view class="col-24 bg-tawny padding-sm">
								24
							</view>
						</view>
						<view class="row margin-xs">
							<view class="col-12 bg-brown  padding-sm">
								12
							</view>
							<view class=" col-12 bg-tawny  padding-sm">
								12
							</view>
							<view class="col-12 bg-brown  padding-sm">
								12
							</view>
							<view class=" col-12 bg-tawny  padding-sm">
								12
							</view>
						</view>
						<view class="row margin-xs">
							<view class="col-8 bg-brown  padding-sm">
								8
							</view>
							<view class="col-8 bg-tawny  padding-sm">
								8
							</view>
							<view class="col-8 bg-brown  padding-sm">
								8
							</view>
							<view class="col-8 bg-tawny  padding-sm">
								8
							</view>
							<view class="col-8 bg-brown  padding-sm">
								8
							</view>
							<view class="col-8 bg-tawny  padding-sm">
								8
							</view>
						</view>
						<view class="row margin-xs">
							<view class="col-6 bg-brown  padding-sm">
								6
							</view>
							<view class=" col-6 bg-tawny  padding-sm">
								6
							</view>
							<view class="col-6 bg-brown  padding-sm">
								6
							</view>
							<view class="col-6 bg-tawny  padding-sm">
								6
							</view>
							<view class="col-6 bg-brown  padding-sm">
								6
							</view>
							<view class="col-6 bg-tawny  padding-sm">
								6
							</view>
							<view class="col-6 bg-brown  padding-sm">
								6
							</view>
							<view class="col-6 bg-tawny  padding-sm">
								6
							</view>
						</view>
						<view class="row justify-around margin-xs">
							<view class="col-4 bg-brown  padding-sm">
								6
							</view>
							<view class="col-6 bg-tawny  padding-sm">
								6
							</view>
							<view class="col-8 bg-brown  padding-sm">
								8
							</view>

						</view>

					</view>
				</view>
				<!-- 等分列 end-->
				<!-- 等高 start-->
				<view class="fui-car wrap-item margin-top-xl  shadow radius">
					<view class="fui-car__header padding-sm margin-xs">
						<image src="../../static/images/icons/dg.png" mode=""></image>
						等高
					</view>
					<view class="fui-car__content padding-sm ">
						<view class="row margin-xs square-4 justify-between">
							<view class=" bg-orange ">

							</view>
							<view class=" bg-tawny ">

							</view>
							<view class=" bg-brown ">

							</view>
							<view class=" bg-tawny ">

							</view>
						</view>

					</view>
				</view>
				<!-- 等高 end-->
			</view>
			<view v-show="TabIndex==3">
				<!-- 浮动 start-->
				<view class="fui-car wrap-item margin-top-xl  shadow radius">
					<view class="fui-car__header padding-sm margin-xs">
						<image src="../../static/images/icons/gdcc.png" mode=""></image>
						浮动
					</view>
					<view class="fui-car__content padding-sm margin-xs">
						<view class="clear-float ">

							<view class="fl bg-green  padding-sm">
								Leyout fl
							</view>
							<view class="fr bg-green  padding-sm">
								Leyout fr
							</view>

						</view>

					</view>
				</view>
				<!-- 浮动 end-->
				<!-- 内外边距 start-->
				<view class="fui-car wrap-item margin-top-xl  shadow radius">
					<view class="fui-car__header padding-sm margin-xs">
						<image src="../../static/images/icons/czdq.png" mode=""></image>
						内外边距
					</view>
					<view class="fui-car__header padding-sm margin-xs">
						{size}的尺寸有xs/sm/df/lg/xl
					</view>
					<view style="font-size: 26rpx;color:#666666" class="fui-car__content padding-sm margin-xs">
					<view class="flex-wrap line-b padding-tb-sm ">
						<view class="fui-df">
							外边距
						</view>
						<view class="fui-df">
							内边距
						</view>
						<view class="fui-df">
							.margin-{size}
						</view>
						<view class="fui-df">
							.padding-{size}
						</view>
					</view>
					<view class="flex-wrap line-b padding-tb-sm">
						<view class="fui-df">
							水平方向外边距
						</view>
						<view class="fui-df">
							水平方向内边距
						</view>
						<view class="fui-df">
							.margin-lr-{size}
						</view>
						<view class="fui-df">
							.padding-lr-{size}
						</view>
					</view>
					<view class="flex-wrap line-b padding-tb-sm">
						<view class="fui-df">
							垂直方向外边距
						</view>
						<view class="fui-df">
							垂直方向内边距
						</view>
						<view class="fui-df">
							.margin-tb-{size}
						</view>
						<view class="fui-df">
							.padding-tb-{size}
						</view>
					</view>
					<view class="flex-wrap line-b padding-tb-sm">
						<view class="fui-df">
							上外边距
						</view>
						<view class="fui-df">
							上内边距
						</view>
						<view class="fui-df">
							.margin-top-{size}
						</view>
						<view class="fui-df">
							.padding-top-{size}
						</view>
					</view>
					<view class="flex-wrap line-b padding-tb-sm">
						<view class="fui-df">
							右外边距
						</view>
						<view class="fui-df">
							右内边距
						</view>
						<view class="fui-df">
							.margin-right-{size}
						</view>
						<view class="fui-df">
							.padding-right-{size}
						</view>
					</view>
					<view class="flex-wrap line-b padding-tb-sm">
						<view class="fui-df">
							下外边距
						</view>
						<view class="fui-df">
							下内边距
						</view>
						<view class="fui-df">
							.margin-bottom-{size}
						</view>
						<view class="fui-df">
							.padding-bottom-{size}
						</view>
					</view>
					<view class="flex-wrap  padding-tb-sm">
						<view class="fui-df">
							左外边距
						</view>
						<view class="fui-df">
							左内边距
						</view>
						<view class="fui-df">
							.margin-left-{size}
						</view>
						<view class="fui-df">
							.padding-left-{size}
						</view>
					</view>
					</view>
				</view>
				<!-- 内外边距 end-->
			</view>
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
				TabIndex: 3
			}
		},
		methods: {
			onTopTab(index) {
				this.TabIndex = index
			}
		}
	}
</script>

<style>
</style>
