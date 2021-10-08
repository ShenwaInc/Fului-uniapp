<template>
	<view class="content">
		<Element v-if="page=='Element'"></Element>
		<Comp v-if="page=='Component'"></Comp>
		<Extend v-if="page=='Extend'"></Extend>
		<About v-if="page=='About'"></About>
		<view class="foot">
			<view  @click="footChange" data-page='Element'>
				<view class="fui-icon">
					<image :src="'../static/images/icons/'+[page=='Element'?'yuansu2':'yuansu1']+'.png'" mode=""></image>
				</view>
				<view class=" icon-font " :class="{activate:page=='Element'}">
					元素
				</view>
			</view>
			<view class="" @click="footChange" data-page="Component">
				<view class="fui-icon">
					<image :src="'../static/images/icons/'+[page=='Component'?'zujian2':'zujian1']+'.png'" mode=""></image>
				</view>
				<view class="icon-font" :class="{activate:page=='Component'}">
					组件
				</view>
			</view>
			<view class="" @click="footChange" data-page="Extend">
				<view class="fui-icon">
					<image :src="'../static/images/icons/'+[page=='Extend'?'kuozhan2':'kuozhan1']+'.png'" mode=""></image>
				</view>
				<view class="icon-font" :class="{activate:page=='Extend'}">
					扩展
				</view>
			</view>
			<view class="" @click="footChange" data-page="About">
				<view class="fui-icon">
					<image :src="'../static/images/icons/'+[page=='About'?'guanyu2':'guanyu1']+'.png'" mode=""></image>
				</view>
				<view class="icon-font" :class="{activate:page=='About'}">
					关于
				</view>
			</view>
		</view>
	</view>
</template>

<script>
	import Element from '@/pages/Element/index.vue'
	import Comp from '@/pages/Comp/index.vue'
	import Extend from '@/pages/Extend/index.vue'
	import About from '@/pages/About/index.vue'
	export default {
		components: {
			Element,Comp,Extend,About
		},
		data() {
			return {
				page:'Element'
			}
		},
		onLoad() {

		},
		//onLaunch、onShow、onHide

		methods: {
			footChange(e){
				this.page=e.currentTarget.dataset.page
			}
		}
	}
</script>

<style lang="scss">
	
</style>
