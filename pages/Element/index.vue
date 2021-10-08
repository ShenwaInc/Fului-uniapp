<template>
	<view class="wrap">
		<view class="title">
			{{data.Title}}
		</view>
		<view class="nav-list">
			<view class="nav-item" v-for="(item,index) in data.itemList" :key="index" @tap="goPage(item.itemText)">
				<view class="item-img">
					<image :src="item.itemImgUrl" mode=""></image>
				</view>
				<view class="">
					<view class="item-title">
						{{item.itemTitle}}
					</view>
					<view class="item-text">
						{{item.itemText}}
					</view>
				</view>
			</view>

		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				data: {
					Title: '交互组件',
					itemList: [{
							itemTitle: '布局',
							itemText: "Layout",
							itemImgUrl: '../static/images/icons/Layout.png'

						},
						{
							itemTitle: '背景',
							itemText: "Bg",
							itemImgUrl: '../static/images/icons/Bg.png'

						},
						{
							itemTitle: '标签',
							itemText: "Tag",
							itemImgUrl: '../static/images/icons/Tag.png'

						},
						{
							itemTitle: '图标',
							itemText: "Icon",
							itemImgUrl: '../static/images/icons/Icon.png'

						},
						{
							itemTitle: '按钮',
							itemText: "Button",
							itemImgUrl: '../static/images/icons/Button.png'

						},
						{
							itemTitle: '文本',
							itemText: "Text",
							itemImgUrl: '../static/images/icons/Text.png'

						},
						{
							itemTitle: '边框阴影',
							itemText: "Shadow",
							itemImgUrl: '../static/images/icons/Shadow.png'

						},
						{
							itemTitle: '加载',
							itemText: "loading",
							itemImgUrl: '../static/images/icons/loading.png'

						},
						{
							itemTitle: '头像',
							itemText: "Avatar",
							itemImgUrl: '../static/images/icons/Avatar.png'

						},
						{
							itemTitle: '进度条',
							itemText: "Process",
							itemImgUrl: '../static/images/icons/Process.png'

						}
					]
				}
			}
		},
		methods: {
			goPage(page) {
				uni.navigateTo({
					url:'/pages/Element/'+page
				})
			}
		}
	}
</script>

<style>
</style>
