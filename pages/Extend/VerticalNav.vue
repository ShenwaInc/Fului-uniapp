<template>
	<view class="">
		<FuiNavBar class="bg-blue"> 
			<block slot="title">垂直导航</block>
		</FuiNavBar>
		<view class="fui-vertical">
			<scroll-view class="fui-vertical__nav" scroll-y scroll-with-animation :scroll-top="verticalNavTop" style="height:calc(100vh - 180rpx)">
				<view class="verticalNav-item" :class="{'activate':tabCur==index}" v-for="(item,index) in 10" :key="index" @tap="TabSelect"
				 :data-id="index">
					选项{{item}}
				</view>
			</scroll-view>
			<scroll-view class="VerticalMain" scroll-y scroll-with-animation style="height:calc(100vh - 180rpx)"
			 :scroll-into-view="'main-'+mainCur" @scroll="VerticalMain">
				<view class="padding-lr-df padding-top-xl" v-for="(item,index) in 10" :key="index" :id="'main-'+index">
					<view class="fui-car wrap-item shadow radius bg-white">
						<view class="fui-car__content ">
							<image style="width:100%;height: 240rpx;" src="../../static/images/icons/card1.png" mode=""></image>
						</view>
						<view class="fui-car__foot flex padding-sm margin-xs">
							<image class="fui-avatar xl round" src="../../static/images/icons/txcxxz2.png" mode=""></image>
							<view class="flex-column justify-around margin-left-xl">
								<text>Adelaide Ramos</text>
								<text class="font-xs text-grey">24天前</text>
							</view>
						</view>
					</view>
					
				</view>
			</scroll-view>
		</view>
	</view>
</template>

<script>
	import FuiNavBar from '@/common/FuiNavBar.vue'
	export default{
		components:{FuiNavBar},
		data(){
			return{
				tabCur: 0,
				mainCur: 0,
				verticalNavTop: 0,
			}
		},
		onLoad() {
			let list = [{}];
			for (let i = 0; i < 26; i++) {
				list[i] = {};
				list[i].name = String.fromCharCode(65 + i);
				list[i].id = i;
			}
			this.list = list;
			this.listCur = list[0];
		},
		methods: {
			TabSelect(e) {
				this.tabCur = e.currentTarget.dataset.id;
				this.mainCur = e.currentTarget.dataset.id;
				this.verticalNavTop = (e.currentTarget.dataset.id - 1) * 50
			},
			VerticalMain(e) {
				// #ifdef MP-ALIPAY
				   return false  //支付宝小程序暂时不支持双向联动 
				// #endif
				let that = this;
				let tabHeight = 0;
				if (this.load) {
					for (let i = 0; i < this.list.length; i++) {
						let view = uni.createSelectorQuery().select("#main-" + this.list[i].id);
						view.fields({
							size: true
						}, data => {
							this.list[i].top = tabHeight;
							tabHeight = tabHeight + data.height;
							this.list[i].bottom = tabHeight;
						}).exec();
					}
					this.load = false
				}
				let scrollTop = e.detail.scrollTop + 10;
				for (let i = 0; i < this.list.length; i++) {
					if (scrollTop > this.list[i].top && scrollTop < this.list[i].bottom) {
						this.verticalNavTop = (this.list[i].id - 1) * 50
						this.tabCur = this.list[i].id
						console.log(scrollTop)
						return false
					}
				}
			}
		},
	}
</script>

<style scoped>

</style>
