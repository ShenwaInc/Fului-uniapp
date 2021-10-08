<template>
	<view class="fui-nav-bar">
		<view @tap="backPage" class="left-arrow"></view>
		<view class="fui-nav-bar__content">
			<slot name="content"></slot>
		</view>
	</view>
</template>

<script>
	export default{
		methods:{
			backPage(){
				uni.navigateBack({
					delta: 1
				})
			}
		}
	}
</script>

<style>
</style>
