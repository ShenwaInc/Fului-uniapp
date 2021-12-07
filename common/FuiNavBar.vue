<template>
	<view class="fui-nav-bar">
		<!-- 	<view @tap="backPage" class="left-arrow"></view> -->
		<view class="fui-nav-bar__left  padding-left-df font-df" @tap="backPage">
			<slot name="left">
				<view class="left-arrow"></view>
			</slot>
		</view>
		<view class="fui-nav-bar__title fui-ellipsis flex-column justify-content align-center">
			<view class="font-xl bold">
				<slot name="title"></slot>
			</view>
			<view class="font-xs">
				<slot name="subtitleTitle"></slot>
			</view>
		</view>
		<view class="fui-nav-bar__right  padding-right-df font-df ">
			<view class="icon">
				<slot name="icon"></slot>
			</view>
			<view class="icon2">
				<slot name="icon2"></slot>
			</view>
		</view>
	</view>
</template>

<script>
	export default {
		props: {


		},
		mounted() {},
		methods: {
			backPage() {
				uni.navigateBack({
					delta: 1
				})
			}
		}
	}
</script>

<style>
</style>
