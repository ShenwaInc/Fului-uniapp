<template>
	<view class="">
		<FuiNavBar class="bg-blue">
			<block slot="title">上传控件</block>
		</FuiNavBar>
		<view class="wrap">
			<!-- 上传样式1 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/czdq.png" mode=""></image>
					上传样式1
				</view>
				<view class="fui-car__content padding-sm margin-xs">
					<view class="flex justify-between padding-bottom-df">
						<text>图片上传</text>
						<text>0/4</text>
					</view>
					<view class="fui-uploader" @tap="Upload">
						<view class="fui-uploader__wrapper">
							<view class="fui-uploader__upload">
								<icon type="search" size="26" />
							</view>
						</view>
					</view>
				</view>
			</view>
			<!-- 上传样式1 end -->
			<!-- 上传样式2 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/czdq.png" mode=""></image>
					上传样式2
				</view>
				<view class="fui-car__content padding-sm margin-xs">
					<view class="flex justify-between padding-bottom-df">
						<text>图片上传</text>

					</view>
					<view class="flex justify-around">
						<view class="fui-uploader" @tap="Upload">
							<view class="fui-uploader__wrapper">
								<view class="fui-uploader__upload bg-darkgrey ">
									<text class="font-df ">上传成功</text>
									<icon class="fui-uploader__clear" type="clear" size="17"  color="#E94F4F"/>
								</view>
							</view>
						</view>
						<view class="fui-uploader" @tap="Upload">
							<view class="fui-uploader__wrapper">
								<view class="fui-uploader__upload bg-bg_grey">
									<icon type="waiting" size="26" />
								</view>
							</view>
						</view>
						<view class="fui-uploader" @tap="Upload">
							<view class="fui-uploader__wrapper">
								<view class="fui-uploader__upload bg-bg_grey">
									<icon type="waiting" size="26" />
								</view>
							</view>
						</view>
					</view>
				</view>
			</view>
			<!-- 上传样式2 end -->
			<!-- 上传样式3 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/czdq.png" mode=""></image>
					上传样式3
				</view>
				<view class="fui-car__content padding-sm margin-xs">
					<view class="fui-uploader" @tap="Upload">
						<view class="fui-uploader__wrapper">
							<view class="fui-uploader__upload fui-upload-3">
								<icon type="search" size="40" />
								<text class="padding-sm">点击上传</text>
								<text class="font-xs text-grey">只能上传jpg/png文件，且不超过2MB</text>
							</view>
						</view>
					</view>
				</view>
			</view>
			<!-- 上传样式3 end -->
			<!-- 上传样式4 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/czdq.png" mode=""></image>
					上传样式4
				</view>
				<view class="fui-car__content padding-sm margin-xs">
					<view class="fui-uploader" @tap="Upload">
						<view class="fui-uploader__wrapper">
							<view class="fui-uploader__upload fui-upload-3">
								<button class="fui-button fui-button-xl primary shadow">点击上传</button>
								<text class="padding-sm">只能上传jpg/png文件，且不超过2MB</text>
								<text class="font-xs text-grey">文件名称.jpg</text>
							</view>
						</view>
					</view>
				</view>
			</view>
			<!-- 上传样式4 end -->
		</view>
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
				Progress: 0,
				url: ''
			}
		},
		methods: {
			async Upload() {
				let [err, image] = await uni.chooseImage()

				console.log("image: ", image);
			}
		}
	}
</script>

<style scoped>
	
</style>
