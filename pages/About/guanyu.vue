<template>
	<view class="">
		<FuiNavBar class="bg-blue">
			<block slot="title">关于</block>
		</FuiNavBar>
		<view class="wrap">
			<!--  start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/czdq.png" mode=""></image>
					关于Fluent Ui组件库
				</view>

				<view class="fui-car__content padding-df">
					<view class="font-df padding-bottom-sm">
						定位“有什么，要什么，放弃什么”，关键的要素“要去做”
					</view>
					<view class="font-df padding-bottom-sm">
						永远不要跟别人比幸运，我从来没想过我比别人幸运，我也许比他们更有毅力，在最困难的时候，他们熬不住了，我可以多熬一秒钟、二秒钟
					</view>
					<view class="font-df padding-bottom-sm">
						高效做好重要和紧急的事情，腾出大量时间做重要不紧要的事情，尽快做好紧急不重要的事情，避免不重要不紧急的事情
					</view>
					<view class="font-df padding-bottom-sm">
						对自己要以身作则；对团队要将心比心；对业务要身先士卒
					</view>
					<view class="font-df padding-bottom-sm">
						当你有一个傻瓜时，你会很痛苦；你有 50 个傻瓜是最幸福的，吃饭、睡觉、上厕所排着队去的；你有一个聪明人时很带劲，你有 50
						个聪明人实际上是最痛苦的，谁都不服谁。我在公司里的作用就象水泥，把许多优秀的人才粘合起来，使他们力气往一个地方使
					</view>
					<view class="font-df padding-bottom-sm">
						一个方案是一流的 idea 加三流的实施；另外一个方案，一流的实施，三流的 idea，哪个好？我选一流的实施，三流的 idea
					</view>
					<view class="font-df padding-bottom-sm">
						事做不做得到，有的时候是听天由命，但是做不做、怎么做那是关键
					</view>
				</view>
			</view>
			<!--  end -->
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
