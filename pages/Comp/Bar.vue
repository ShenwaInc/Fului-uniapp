<template>
	<view class="">
		<FuiNavBar class="bg-blue"> 
			<block slot="title">导航栏</block>
		</FuiNavBar>
		<view class="wrap">
			<!-- 底部操作条 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/czdq.png" mode=""></image>
					底部操作条
				</view>
			
				<view class="fui-car__content padding-sm margin-xs bg-bg_light_gray">
				<!-- 	1、 -->
				<view class="fui-bar flex  padding-tb-sm bg-white  margin-bottom-lg">
					<view  @click="footChange" data-page='Element'>
						<view class="fui-bar-icon">
							<image :src="'../../static/images/icons/'+[page=='Element'?'yuansu2':'yuansu1']+'.png'" mode=""></image>
						</view>
						<view class=" icon-font " :class="{activate:page=='Element'}">
							元素
						</view>
					</view>
					<view class="" @click="footChange" data-page="Component">
						<view class="fui-bar-icon">
							<image :src="'../../static/images/icons/'+[page=='Component'?'zujian2':'zujian1']+'.png'" mode=""></image>
						</view>
						<view class="icon-font" :class="{activate:page=='Component'}">
							组件
						</view>
					</view>
					<view class="" @click="footChange" data-page="Extend">
						<view class="fui-bar-icon">
							<image :src="'../../static/images/icons/'+[page=='Extend'?'kuozhan2':'kuozhan1']+'.png'" mode=""></image>
						</view>
						<view class="icon-font" :class="{activate:page=='Extend'}">
							扩展
						</view>
					</view>
					<view class="" @click="footChange" data-page="About">
						<view class="fui-bar-icon">
							<image :src="'../../static/images/icons/'+[page=='About'?'guanyu2':'guanyu1']+'.png'" mode=""></image>
						</view>
						<view class="icon-font" :class="{activate:page=='About'}">
							关于
						</view>
					</view>
				</view>
				<!-- 	2、 -->
				<view class="fui-bar flex  padding-tb-sm bg-white br-top-radius margin-bottom-lg">
					<view  @click="footChange" data-page='Element'>
						<view class="fui-bar-icon">
							<image :src="'../../static/images/icons/'+[page=='Element'?'yuansu2':'yuansu1']+'.png'" mode=""></image>
						</view>
						<view class=" icon-font " :class="{activate:page=='Element'}">
							元素
						</view>
					</view>
					<view class="" @click="footChange" data-page="Component">
						<view class="fui-bar-icon">
							<image :src="'../../static/images/icons/'+[page=='Component'?'zujian2':'zujian1']+'.png'" mode=""></image>
						</view>
						<view class="icon-font" :class="{activate:page=='Component'}">
							组件
						</view>
					</view>
					<view class="" @click="footChange" data-page="Extend">
						<view class="fui-bar-icon">
							<image :src="'../../static/images/icons/'+[page=='Extend'?'kuozhan2':'kuozhan1']+'.png'" mode=""></image>
						</view>
						<view class="icon-font" :class="{activate:page=='Extend'}">
							扩展
						</view>
					</view>
					<view class="" @click="footChange" data-page="About">
						<view class="fui-bar-icon">
							<image :src="'../../static/images/icons/'+[page=='About'?'guanyu2':'guanyu1']+'.png'" mode=""></image>
						</view>
						<view class="icon-font" :class="{activate:page=='About'}">
							关于
						</view>
					</view>
				</view>
				<!-- 	3、 -->
				<view class="fui-bar flex  padding-tb-sm bg-white br-top-radius margin-bottom-xl">
					<view  @click="footChange" data-page='Element'>
						<view :class="{'fui-bar-dented':page=='Element'}" class="fui-bar-icon ">
							<image :src="'../../static/images/icons/'+[page=='Element'?'yuansu1':'yuansu2']+'.png'" mode=""></image>
						</view>
						<view class=" icon-font " :class="{activate:page=='Element'}">
							元素
						</view>
					</view>
					<view class="" @click="footChange" data-page="Component">
						<view :class="{'fui-bar-dented':page=='Component'}" class="fui-bar-icon">
							<image :src="'../../static/images/icons/'+[page=='Component'?'zujian1':'zujian2']+'.png'" mode=""></image>
						</view>
						<view class="icon-font" :class="{activate:page=='Component'}">
							组件
						</view>
					</view>
					<view class="" @click="footChange" data-page="Extend">
						<view :class="{'fui-bar-dented':page=='Extend'}" class="fui-bar-icon ">
							<image :src="'../../static/images/icons/'+[page=='Extend'?'kuozhan1':'kuozhan2']+'.png'" mode=""></image>
						</view>
						<view class="icon-font" :class="{activate:page=='Extend'}">
							扩展
						</view>
					</view>
					<view class="" @click="footChange" data-page="About">
						<view :class="{'fui-bar-dented':page=='About'}" class="fui-bar-icon">
							<image :src="'../../static/images/icons/'+[page=='About'?'guanyu1':'guanyu2']+'.png'" mode=""></image>
						</view>
						<view class="icon-font" :class="{activate:page=='About'}">
							关于
						</view>
					</view>
				</view>
				<!-- 	4、 -->
				<view class="fui-bar flex  padding-tb-sm bg-white  ">
					<view  @click="footChange" data-page='Element'>
						<view class="fui-bar-icon">
							<image :src="'../../static/images/icons/'+[page=='Element'?'yuansu2':'yuansu1']+'.png'" mode=""></image>
						</view>
						<view class=" icon-font " :class="{activate:page=='Element'}">
							元素
						</view>
					</view>
					<view class="" @click="footChange" data-page="Component">
						<view class="fui-bar-icon">
							<image :src="'../../static/images/icons/'+[page=='Component'?'zujian2':'zujian1']+'.png'" mode=""></image>
						</view>
						<view class="icon-font" :class="{activate:page=='Component'}">
							组件
						</view>
					</view>
					<view class="" @click="footChange" data-page="Publish">
						<view class="fui-bar-icon fui-bar-bulge">
							<image :src="'../../static/images/icons/publish.png'" mode=""></image>
						</view>
						<view class="icon-font" :class="{activate:page=='Component'}">
							发布
						</view>
					</view>
					<view class="" @click="footChange" data-page="Extend">
						<view class="fui-bar-icon ">
							<image :src="'../../static/images/icons/'+[page=='Extend'?'kuozhan2':'kuozhan1']+'.png'" mode=""></image>
						</view>
						<view class="icon-font" :class="{activate:page=='Extend'}">
							扩展
						</view>
					</view>
					<view class="" @click="footChange" data-page="About">
						<view class="fui-bar-icon">
							<image :src="'../../static/images/icons/'+[page=='About'?'guanyu2':'guanyu1']+'.png'" mode=""></image>
						</view>
						<view class="icon-font" :class="{activate:page=='About'}">
							关于
						</view>
					</view>
				</view>
				</view>
			</view>
			<!-- 底部操作条 end -->
			<!-- 顶部导航栏 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/czdq.png" mode=""></image>
					顶部导航栏
				</view>
			
				<view class="fui-car__content padding-sm margin-xs  bg-bg_light_gray">
			
				<FuiNavBar >
					<block slot="title">标准导航栏</block>
				</FuiNavBar>
				<FuiNavBar class="margin-top-sm" >
					<block slot="title">更多按钮导航</block>
					<block slot="icon">...</block>
				</FuiNavBar>
				<FuiNavBar class="margin-top-sm" >
					<block slot="title">文字+icon 导航</block>
					<block slot="icon">账单</block>
					<block slot="icon2">...</block>
				</FuiNavBar>
				<FuiNavBar class="margin-top-sm" >
					<block slot="title">2 icon 导航</block>
					<block slot="icon">+</block>
					<block slot="icon2">...</block>
				</FuiNavBar>
				<FuiNavBar class="margin-top-sm" >
					<block slot="title">主副标题导航栏</block>
					<block slot="subtitleTitle">副标题</block>
					<block slot="icon">...</block>
				</FuiNavBar>
				<FuiNavBar class="margin-top-sm" >
					<block slot="title">可下拉导航栏 v</block>
					<block slot="icon">...</block>
				</FuiNavBar>
				<FuiNavBar class="margin-top-sm" >
					<block slot="left">取消</block>
					<block slot="title">模态导航栏</block>
					<block slot="icon">
						<uni-button class="fui-button fui-button-df bg-royalblue round">完成</uni-button>
					</block>
				</FuiNavBar>
				<FuiNavBar class="margin-top-sm" >
					<block slot="title">
						<view class="margin-lr-xs flex search radius">
							<input type="text" value="" placeholder="搜索词"/>
						</view>
					</block>
					<block slot="icon2">
						<uni-button class="fui-button fui-button-df bg-royalblue round">搜索</uni-button>
					</block>
				</FuiNavBar>
				
				
				</view>
				</view>
			<!-- 顶部导航栏 end -->
		</view>
	</view>
</template>

<script>
	import FuiNavBar from '@/common/FuiNavBar.vue'
	export default{
		components:{FuiNavBar},
		data(){
			return{
				page:'Element'
			}
		},
		methods:{
			footChange(e){
				this.page=e.currentTarget.dataset.page
			}
		}
	}
</script>

<style>
</style>
