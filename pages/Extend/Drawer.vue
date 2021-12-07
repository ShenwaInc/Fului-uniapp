<template>
	<view class="">
		<FuiNavBar class="bg-blue">
			<block slot="title">全屏抽屉</block>
		</FuiNavBar>
		<view class="wrap">
			<!-- 图标 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/czdq.png" mode=""></image>
					全屏抽屉
				</view>

				<view class="fui-car__content padding-lr-sm margin-xs">

					<view class="fui-drawer">
						<view :class="{'activate':drawerIndex==item}" @tap="drawerIndex=drawerIndex==item?0:item"
							v-for="item in 10" :key="item">
							<view class="flex align-center justify-between padding-tb-sm line-b">
								<view class="flex">
									<view class="icon">
										icon
									</view>
									<text class="padding-left-sm">标题{{item}}</text>
								</view>
								<view class="right-arrow margin-right-lg">
								</view>
							</view>
							<view :class="'drawer-'+item"  class="fui-drawer__content  ">
								<view style="text-indent: 2em;">
									不要再纠缠于“长期”和“短期”，很多时候长期已经成为了现在不做事情的借口
								</view>
								<view style="text-indent: 2em;">说出来的是你想的，做出来的是你说的，交出来的是你做的</view>
							</view>
						</view>

					</view>

				</view>
			</view>
			<!-- 图标 end -->
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
				drawerIndex: 1,
			}
		},
		mounted(){

			// uni.createSelectorQuery().select(".drawer-1").boundingClientRect(res=>{
			// 	console.log('111',res.height)
			// }).exec()
		}
	}
</script>

<style scoped>
	.icon {
		width: 25px;
		height: 25px;
		background: #D8D8D8;
		/* #2C5EC2 */
		border-radius: 50%;
		font-size: 10px;
		display: flex;
		align-items: center;
		color: #fff;
		transition: .6s;
	}


	
</style>
