<template>
	<view class="">
		<FuiNavBar class="bg-blue">
			<block slot="title">文本</block>
		</FuiNavBar>
		<view class="wrap">
			<!-- 单行文本框1 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/czdq.png" mode=""></image>
					单行文本框1
				</view>
				<view class="fui-car__content padding-lr-sm margin-xs fui-form-group">
					<view class="fui-form">
						<view class="lable">字段</view>
						<input type="text" placeholder="请输入内容" />
					</view>
					<view class="fui-form">
						<view class="lable">收获地址</view>
						<input type="text" placeholder="输入框带图标" />
						<image class="fui-avatar sm round bg-white" src="../../static/images/icons/dizhi.png" mode="">
						</image>
					</view>
					<view class="fui-form">
						<view class="lable">身份证号</view>
						<input type="text" placeholder="输入框长度限制" />
						<view class="text-grey">
							0/18
						</view>
					</view>
					<view class="fui-form">
						<view class="lable">字段</view>
						<input type="text" placeholder="输入内容可清空" />
						<image class="fui-avatar sm round bg-DeepSkyBlue" src="../../static/images/icons/jzerror.png"
							mode=""></image>
					</view>
					<view class="fui-form">
						<view class="lable">验证码</view>
						<input type="text" placeholder="输入框带按钮" />
						<uni-button class="fui-button fui-button-df bg-blue">验证码</uni-button>
					</view>
				</view>
			</view>
			<!-- 单行文本框1 end -->

			<!-- 单行文本框2 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/czdq.png" mode=""></image>
					单行文本框2
				</view>
				<view class="fui-car__content padding-lr-sm margin-xs ">
					<view class="fui-form solid">
						<view class="lable">字段</view>
						<input type="text" placeholder="请输入内容" />
					</view>
					<view class="fui-form solid">
						<view class="lable">禁用字段</view>
						<input class="fui-input" disabled type="text" placeholder="请输入内容" />
					</view>
					<view class="fui-form solid">
						<view class="lable">可清空字段</view>
						<input type="text" placeholder="请输入内容" />
						<view class="fui-form__icon">
							<image class="fui-avatar sm round bg-DeepSkyBlue"
								src="../../static/images/icons/jzerror.png" mode=""></image>
						</view>
					</view>
				</view>
			</view>
			<!-- 单行文本框2 end -->
			<!-- 单行文本框3 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/czdq.png" mode=""></image>
					单行文本框3
				</view>
				<view class="fui-car__content padding-lr-sm margin-xs ">
					<view class="padding-tb-xs">输入框</view>
					<view class="  fui-form solid">
						<input type="text" placeholder="请输入内容" />
					</view>

					<view class="padding-tb-xs">输入框带图标按钮</view>
					<view class="  fui-form solid">
						<input class="fui-form__checked" type="text" placeholder="请选择日期" />
						<view class="fui-form__icon">
							<image class="fui-avatar sm round bg-DeepSkyBlue"
								src="../../static/images/icons/jzerror.png" mode=""></image>
						</view>
					</view>

					<view class="padding-tb-xs">输入框错误</view>
					<view class="  fui-form solid ">
						<input class="fui-form__error" type="text" placeholder="请输入内容" />
						<view class="fui-form__tip font-sm">
							输入错误
						</view>
					</view>

					<view class="padding-tb-xs">输入框通过</view>
					<view class="  fui-form solid ">
						<input class="fui-form__success" type="text" placeholder="输入成功" />
						<view class="fui-form__icon">
							<image class="fui-avatar sm round bg-DeepSkyBlue" src="../../static/images/icons/jdt.png"
								mode=""></image>
						</view>
					</view>
				</view>
			</view>
			<!-- 单行文本框3 end -->
			<!-- 复合型文本框 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/czdq.png" mode=""></image>
					复合型文本框
				</view>
				<view class="fui-car__content padding-lr-sm margin-xs ">

					<view class="fui-form solid">
						<view class="bg-bg_grey padding-tb-sm">https://</view>
						<input type="text" placeholder="请输入内容" />
					</view>
					<view class="fui-form solid">

						<input type="text" placeholder="请输入内容" />
						<view class="bg-bg_grey padding-tb-sm"> .com </view>
					</view>

					<view class="fui-form solid">
						<view class="bg-bg_grey padding-tb-sm">请选择 V</view>
						<input type="text" placeholder="请输入证件号码" />
					</view>




				</view>
			</view>
			<!-- 复合型文本框 end -->
			<!-- 多行文本框 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/czdq.png" mode=""></image>
					多行文本框
				</view>
				<view class="fui-car__content padding-lr-sm margin-xs ">
					<view class="fui-textarea ">
						<text>描述信息</text>
						<textarea value="" class="bg-white" placeholder="请输入长文本内容" />
					</view>
					<view class="fui-textarea flex margin-top-df">
						<text >描述信息</text>
						<textarea value="" class="bg-bg_light_gray" placeholder="请输入内容" />
					</view>
					<view class="fui-textarea flex-column margin-top-df">
						<text >描述信息</text>
						<textarea value="" class="bg-bg_light_gray" placeholder="请输入内容" />
					</view>
					

				</view>
			</view>
			<!-- 多行文本框 end -->
		</view>
	</view>
</template>

<script>
	import FuiNavBar from '@/common/FuiNavBar.vue'
	export default {
		components: {
			FuiNavBar
		}
	}
</script>

<style>
</style>
