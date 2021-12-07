<template>
	<view class="">
		<FuiNavBar class="bg-blue">
			<block slot="title">文本</block>
		</FuiNavBar>
		<!-- 全屏限高轮播 start -->
		<view class="fui-car__header padding-sm  bg-white">
			<image src="../../static/images/icons/czdq.png" mode=""></image>
			全屏限高轮播
		</view>
		<swiper class="fui-swiper-screen" :indicator-dots="true" :autoplay="true" :interval="1000" :duration="500">
			<swiper-item v-for="(item,i) in 5" :key="i">
				<view style="background-color:#4CD964;height: 300px;">{{item}}</view>
			</swiper-item>

		</swiper>
		<!-- 全屏限高轮播 end -->
		<!-- 卡片式轮播 start -->
		<view class="fui-car__header padding-sm  bg-white">
			<image src="../../static/images/icons/czdq.png" mode=""></image>
			卡片式轮播
		</view>
		<swiper class="fui-swiper-card" :indicator-dots="true" :autoplay="true" :interval="5000" :duration="500"
			@change="changeSwiper" :circular="true">
			<swiper-item v-for="(item,i) in 5" :key="i" :class="{'current':cardIndex==i}">
				<view class="fui-swiper__item" style="background-color:#4CD964;height: 150px;">{{item}}</view>
			</swiper-item>
		</swiper>
		<!-- 卡片式轮播 end -->
		<!-- 堆叠式轮播 start -->
		<view class="fui-car__header padding-sm  bg-white">
			<image src="../../static/images/icons/czdq.png" mode=""></image>
			堆叠式轮播
		</view>
		<view class="fui-swiper-stack" @touchmove="TowerMove" @touchstart="TowerStart" @touchend="TowerEnd">
			<view class="tower-item" :class="item.zIndex==1?'none':''" v-for="(item,index) in swiperList" :key="index"
				:style="[{'--index': item.zIndex,'--left':item.mLeft}]" :data-direction="direction">
				<view class="fui-swiper__item">
					<image :src="item.url" mode="aspectFill"></image>
				</view>
			</view>
		</view>
		<!-- 堆叠式轮播 end -->

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
				cardIndex: 0,
				towerStart: 0,
				direction: '',
				swiperList: [{
					id: 0,
					type: 'image',
					url: 'https://ossweb-img.qq.com/images/lol/web201310/skin/big84000.jpg'
				}, {
					id: 1,
					type: 'image',
					url: 'https://ossweb-img.qq.com/images/lol/web201310/skin/big37006.jpg',
				}, {
					id: 2,
					type: 'image',
					url: 'https://ossweb-img.qq.com/images/lol/web201310/skin/big39000.jpg'
				}, {
					id: 3,
					type: 'image',
					url: 'https://ossweb-img.qq.com/images/lol/web201310/skin/big10001.jpg'
				}, {
					id: 4,
					type: 'image',
					url: 'https://ossweb-img.qq.com/images/lol/web201310/skin/big25011.jpg'
				}, {
					id: 5,
					type: 'image',
					url: 'https://ossweb-img.qq.com/images/lol/web201310/skin/big21016.jpg'
				}, {
					id: 6,
					type: 'image',
					url: 'https://ossweb-img.qq.com/images/lol/web201310/skin/big99008.jpg'
				}],
			}
		},
		onLoad() {
			this.TowerSwiper('swiperList');
			// 初始化towerSwiper 传已有的数组名即可
		},
		methods: {
			changeSwiper({
				detail: {
					current
				}
			}) {
				console.log(current)
				this.cardIndex = current
			},
			// towerSwiper
			// 初始化towerSwiper
			TowerSwiper(name) {
				let list = this[name];
				for (let i = 0; i < list.length; i++) {
					list[i].zIndex = parseInt(list.length / 2) + 1 - Math.abs(i - parseInt(list.length / 2))
					list[i].mLeft = i - parseInt(list.length / 2)
				}
				this.swiperList = list
			},
			// towerSwiper触摸开始
			TowerStart(e) {
				this.towerStart = e.touches[0].pageX
			},

			// towerSwiper计算方向
			TowerMove(e) {
				this.direction = e.touches[0].pageX - this.towerStart > 0 ? 'right' : 'left'
			},

			// towerSwiper计算滚动
			TowerEnd(e) {
				let direction = this.direction;
				let list = this.swiperList;
				if (direction == 'right') {
					let mLeft = list[0].mLeft;
					let zIndex = list[0].zIndex;
					for (let i = 1; i < this.swiperList.length; i++) {
						this.swiperList[i - 1].mLeft = this.swiperList[i].mLeft
						this.swiperList[i - 1].zIndex = this.swiperList[i].zIndex
					}
					this.swiperList[list.length - 1].mLeft = mLeft;
					this.swiperList[list.length - 1].zIndex = zIndex;
				} else {
					let mLeft = list[list.length - 1].mLeft;
					let zIndex = list[list.length - 1].zIndex;
					for (let i = this.swiperList.length - 1; i > 0; i--) {
						this.swiperList[i].mLeft = this.swiperList[i - 1].mLeft
						this.swiperList[i].zIndex = this.swiperList[i - 1].zIndex
					}
					this.swiperList[0].mLeft = mLeft;
					this.swiperList[0].zIndex = zIndex;
				}
				this.direction = ""
				this.swiperList = this.swiperList
			},
		}
	}
</script>

<style>


	
</style>
