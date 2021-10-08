<template>
	<view class="wrap">
		<view class="title">
			{{data.Title}}
		</view>
		<view class="extebdList">
			<view :style="{backgroundColor:item.bgColor}" class="extebd-item" v-for="(item,index) in data.itemList" :key="index">
				<view class="extebd-img">
					<image :style="{width:item.imgW+'px',height:item.imgH+'px'}" :src="item.itemImgUrl" mode=""></image>
				</view>
				<view class="extebd-title">
					{{item.itemTitle}}
				</view>
				<view class="extebd-text">
					{{item.itemText}}
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
					Title: '插件扩展',
					itemList: [{
							itemTitle: '索引列表',
							itemText: "Index",
							itemImgUrl: '../static/images/icons/Index.png',
							bgColor: '#2754AD',
							imgW:56,
							imgH:50,
						},
						{
							itemTitle: '全屏抽屉',
							itemText: "Drawer",
							itemImgUrl: '../static/images/icons/Drawer.png',
							bgColor: '#1D9145',
							imgW:46,
							imgH:54,
						},
						{
							itemTitle: '上传控件',
							itemText: "Upload",
							itemImgUrl: '../static/images/icons/Upload.png',
							bgColor: '#BF2A3E',
							imgW:68,
							imgH:48,
						},
						{
							itemTitle: '垂直导航',
							itemText: "Vertical Nav",
							itemImgUrl: '../static/images/icons/Vertical_Nav.png',
							bgColor: '#7B31A3',
							imgW:41,
							imgH:57,
						}
					]
				}
			}
		}
	}
</script>

<style>
</style>
