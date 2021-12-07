<template>
	<view class="about">
		<view class="wrap">
			<view class="about-title">
				Fluent Design UI
			</view>
			<view class="about-text">
				组件库
			</view>
			<view class="about-box">
				<view class="box">
					<view class="box-title">
						14.1W
					</view>
					<view class="box-text">
						View
					</view>
				</view>
				<view class="box">
					<view class="box-title">
						2.0W
					</view>
					<view class="box-text">
						Star
					</view>
				</view>
				<view class="box">
					<view class="box-title">
						1.9K
					</view>
					<view class="box-text">
						Fork
					</view>
				</view>
			</view>
			<view class="abouList">
				<view class="about-item" v-for="(item,index) in itemList" :key="index" @tap="goPage(item.page)">
					<image :src="item.icon" mode=""></image>
					<view class="about-item-text">
						{{item.title}}
					</view>
					<view class="right-arrow padding-right-lg"></view>
				</view>
				
			</view>
		</view>
	</view>

</template>

<script>
	export default {
		data() {
			return {
				itemList: [{
					icon: '../static/images/icons/guanyu.png',
					title: '关于我们',
					page:'guanyu'
					
				}, {
					icon: '../static/images/icons/tuiguang.png',
					title: '推广中心'
				}, {
					icon: '../static/images/icons/lianxi.png',
					title: '联系客服'
				}, {
					icon: '../static/images/icons/yijian.png',
					title: '意见反馈',
					page:'yijian'
				}]
			}
		},methods: {
			goPage(page) {
				uni.navigateTo({
					url:'/pages/About/'+page
				})
			}
		}
	}
</script>

<style>

</style>
