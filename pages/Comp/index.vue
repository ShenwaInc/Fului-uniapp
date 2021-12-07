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
							itemTitle: '导航栏',
							itemText: "Bar",
							itemImgUrl: '../static/images/icons/Bar.png'

						},
						{
							itemTitle: '选项卡',
							itemText: "Nav",
							itemImgUrl: '../static/images/icons/Nav.png'

						},
						{
							itemTitle: '列表',
							itemText: "List",
							itemImgUrl: '../static/images/icons/List.png'

						},
						{
							itemTitle: '卡片',
							itemText: "Card",
							itemImgUrl: '../static/images/icons/Card.png'

						},
						{
							itemTitle: '表单',
							itemText: "Form",
							itemImgUrl: '../static/images/icons/Form.png'

						},
						{
							itemTitle: '时间轴',
							itemText: "Timeline",
							itemImgUrl: '../static/images/icons/Timeline.png'

						},
						{
							itemTitle: '聊天',
							itemText: "Chat",
							itemImgUrl: '../static/images/icons/Chat.png'

						},
						{
							itemTitle: '轮播',
							itemText: "Swiper",
							itemImgUrl: '../static/images/icons/Swiper.png'

						},
						{
							itemTitle: '模态框',
							itemText: "Modal",
							itemImgUrl: '../static/images/icons/Modal.png'

						},
						{
							itemTitle: '步骤条',
							itemText: "Step",
							itemImgUrl: '../static/images/icons/Step.png'

						}
					]
				}
			}
		},
		methods: {
			goPage(page) {
				uni.navigateTo({
					url:'/pages/Comp/'+page
				})
			}
		}
	}
</script>

<style>

</style>
