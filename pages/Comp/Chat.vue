<template>
	<view class="">
		<FuiNavBar class="bg-blue">
			<block slot="title">聊天</block>
		</FuiNavBar>
		<view class="fui-chat">
			<view class="fui-item">
				<view class="time">
					上午10:26
				</view>
				<image class="fui-avatar shadow" src="../../static/images/icons/txcxxz2.png" mode=""></image>
				<view class="info-wrap">
					<view class="info">
						平凡人做非凡事。
					</view>
				</view>
			</view>
			<view class="fui-item">
				<image class="fui-avatar shadow" src="../../static/images/icons/txcxxz2.png" mode=""></image>
				<view class="info-wrap">
					<view class="info">
						🥵
					</view>
				</view>
			</view>
			<view class="fui-chat__tips">
				对方拒绝了你的消息
			</view>
			<view class="fui-item self">
				<view class="info-wrap">
					<view class="info">
						当你只是需要一根针时，千万不要去磨铁棒。
					</view>

				</view>
				<image class="fui-avatar shadow" src="../../static/images/icons/txcxxz1.png" mode=""></image>
			</view>

			<view class="fui-item self">
				<view class="info-wrap">
					<image style="width: 200px;" src="../../static/images/icons/card1.png" mode="widthFix"></image>
				</view>
				<image class="fui-avatar shadow" src="../../static/images/icons/txcxxz1.png" mode=""></image>
			</view>
			<view class="fui-chat__tips">
				对方开启了好友验证，你还不是他 (她)的好友。请先发送好友验证请 求，对方验证通过后，才能聊天。
				<text class="text-blue">发送好友验证</text>
			</view>
			<view class="fui-item">
				<image class="fui-avatar shadow" src="../../static/images/icons/txcxxz2.png" mode=""></image>
				<view class="info-wrap">
					<view class="info">
						<image class="fui-avatar sm bg-white margin-left-xl" src="../../static/images/icons/yuyin.png"
							mode=""></image>
					</view>
					<view class="describe">
						3″
					</view>
				</view>
			</view>
			<view class="fui-item self">
				<view class="info-wrap">
					<image style="width: 200px;" src="../../static/images/icons/card1.png" mode="widthFix"></image>
				</view>
				<image class="fui-avatar shadow" src="../../static/images/icons/txcxxz1.png" mode=""></image>
			</view>
			
		</view>
		<view class="fui-chat__bar padding-xs">
			<image @click="voice" class="fui-avatar sm bg-white margin-left-sm" src="../../static/images/icons/yuyin.png"mode=""></image>
			<image class="fui-avatar sm bg-white margin-left-sm" src="../../static/images/icons/yuyin.png"mode=""></image>
			<view class="flex fui-one align-center" v-show="!voiceMode">
				<input style="height:35px;" class="bg-white line-b margin-left-sm" type="text" value="" />
				<uni-button  class="fui-button fui-button-df bg-green margin-left-sm ">发送</uni-button>
			</view>
			<uni-button @click="onVoic"  v-show="voiceMode" class="fui-button fui-button-df bg-white margin-left-sm fui-one">按住 说话</uni-button>
			<image class="fui-avatar sm bg-white margin-left-sm " src="../../static/images/icons/yuyin.png"mode=""></image>
		</view>
	</view>
</template>

<script>
	import FuiNavBar from '@/common/FuiNavBar.vue'
	export default {
		components: {
			FuiNavBar
		},
		data(){
			return{
				voiceMode:false
			}
		},
		methods:{
			voice(){
				this.voiceMode=!this.voiceMode
			},
			onVoic(){
				uni.showModal({
					content: '语音模态框',
					showCancel: true
				});
			}
		}
	}
</script>

<style>
</style>
