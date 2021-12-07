<template>
	<view class="">
		<FuiNavBar class="bg-blue">
			<block slot="title">模态框</block>
		</FuiNavBar>
		<view class="wrap">
			<!-- 弹出层 start -->
			<view class="fui-car wrap-item margin-top-xl  shadow radius">
				<view class="fui-car__header padding-sm margin-xs">
					<image src="../../static/images/icons/czdq.png" mode=""></image>
					弹出层
				</view>

				<view class="fui-car__content padding-sm margin-xs ">
					<button @tap="showModal" data-name="Modal"
						class="fui-button fui-button-xl margin-tb-df bg-teal">普通窗口</button>
					<view :class="{show:modalName=='Modal'}" class="fui-modal">
						<view class="fui-dialog">
							<view class="fui-dialog__header">
								标题
							</view>
							<view class="fui-dialog__content">
								告知当前状态，信息和解决方
							</view>
							<view class="fui-dialog__footer">
								<button class="fui-button fui-button-xl bg-white text-blue"
									@tap="closeModal">确定</button>
							</view>
						</view>
					</view>
					<button @tap="showModal" data-name="bottomModal"
						class="fui-button fui-button-xl margin-tb-df bg-teal">底部窗口</button>
					<view :class="{show:modalName=='bottomModal'}" class="fui-modal fui-modal--bottom">
						<view class="fui-dialog ">
							<view class="fui-dialog__footer padding-sm flex justify-between">
								<text @tap="closeModal" class="text-blue">确定</text>
								<text @tap="closeModal" class="text-grey">取消</text>

							</view>

							<view class="fui-dialog__content">
								告知当前状态，信息和解决方
							</view>

						</view>
					</view>
					<button @tap="showModal" data-name="dialogModal"
						class="fui-button fui-button-xl margin-tb-df bg-teal">对话窗口</button>
					<view :class="{show:modalName=='dialogModal'}" class="fui-modal">
						<view class="fui-dialog">
							<view class="fui-dialog__header">
								标题单行
							</view>
							<view class="fui-dialog__content">
								<view class="fui-form solid">
									<input type="text" placeholder="您的姓名" />
								</view>
							</view>
							<view class="fui-dialog__footer">
								<button class="fui-button fui-button-xl primary " @tap="closeModal">提交</button>
							</view>
						</view>
					</view>
					<button @tap="showModal" data-name="imgModal"
						class="fui-button fui-button-xl margin-tb-df bg-teal">图片窗口</button>
					<view :class="{show:modalName=='imgModal'}" class="fui-modal">
						<view class="fui-dialog">

							<image style="height: 200px;
    width: 100%;" src="../../static/images/icons/tupian.png" mode=""></image>

							<view class="fui-dialog__header">
								标题
							</view>
							<view class="fui-dialog__content">
								告知当前状态，信息和解决方
							</view>
							<view class="fui-dialog__footer">
								<button class="fui-button fui-button-xl bg-white text-blue"
									@tap="closeModal">确定</button>
							</view>
						</view>
					</view>
					<button @tap="showModal" data-name="radioModal"
						class="fui-button fui-button-xl margin-tb-df bg-teal">单选窗口</button>
					<view :class="{show:modalName=='radioModal'}" class="fui-modal">
						<view class="fui-dialog">
							<view class="fui-dialog__header">
								标题
							</view>
							<view class="fui-dialog__content">
								<view class="flex justify-content">
									<view v-for="item in 4" :key="item" class="fui-tag round primary ">选项</view>
								</view>
							</view>
							<view class="fui-dialog__footer">
								<button class="fui-button fui-button-xl bg-white text-blue"
									@tap="closeModal">提交</button>
							</view>
						</view>
					</view>
					<button @tap="showModal" data-name="checkModal"
						class="fui-button fui-button-xl margin-tb-df bg-teal">多选窗口</button>
					<view :class="{show:modalName=='checkModal'}" class="fui-modal">
						<view class="fui-dialog">
							<view class="fui-dialog__header">
								标题
							</view>
							<view class="fui-dialog__content">
								
									<checkbox-group class="flex-column">
										<label>
											<checkbox value="cb" checked="true" />选项字段，选项字段
										</label>
										<label>
											<checkbox value="cb" />选项字段，选项字段
										</label>
										<label>
											<checkbox value="cb" />选项字段，选项字段
										</label>
									</checkbox-group>						
							</view>
							<view class="fui-dialog__footer">
								<button class="fui-button fui-button-xl bg-white text-blue"
									@tap="closeModal">提交</button>
							</view>
						</view>
					</view> 
					<button @tap="showModal" data-name="drawerModal" class="fui-button fui-button-xl margin-tb-df bg-teal">侧边抽屉</button>
					<view :class="{show:modalName=='drawerModal'}" class="fui-modal drawer" @tap="closeModal">
						<view @tap.stop="" class="fui-dialog">
							<view v-for="item in 6" :key="item" class="fui-cell padding-xs margin-bottom-xs bg-bg_grey">
								<view class="fui-cell__title">
									基础列表{{item}}
								</view>
								<view class="right-arrow"></view>
							</view>
						</view>
					</view>
				</view>
			</view>
			<!-- 弹出层 end -->
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
				modalName: null
			}
		},
		methods: {
			showModal({
				currentTarget: {
					dataset: {
						name
					}
				}
			}) {
				console.log(name)
				this.modalName = name
			},
			closeModal() {
				this.modalName = null
			}
		}
	}
</script>

<style>
	.fui-modal {
		position: fixed;
		top: 0;
		bottom: 0;
		left: 0;
		right: 0;
		z-index: 999;
		background: rgba(0, 0, 0, 0.6);
		transform: scale(2);
		transition: all .3s;
		opacity: 0;
		pointer-events: none;
		display: flex;
		justify-content: center;
		align-items: center;

	}

	.fui-modal.show {

		transform: scale(1);
		transition: all .3s;
		opacity: 1;
		pointer-events: auto;
		overflow-x: hidden;
		overflow-y: auto;
	}

	.fui-dialog {
		width: 540rpx;
		background-color: #fff;
		border-radius: 6rpx;
		text-align: center;
	}

	.fui-dialog__header {
		padding: 48rpx 30rpx 10rpx;
	}

	.fui-dialog__content {
		padding: 10rpx 30rpx 48rpx;
	}


	.fui-dialog__footer {}

	.fui-modal--bottom {
		align-items: flex-end
	}

	.fui-modal--bottom .fui-dialog {
		width: 100%;

	}
	.fui-modal.drawer{
		justify-content: flex-start
	}
	.fui-modal.drawer .fui-dialog {
		width: 460rpx;
		height: 100%;
		border-radius: 0;
		transform: translateX(-100%);
		transition: .5s;
	}
	.fui-modal.show.drawer .fui-dialog {
		transform: translateX(0);
		transition: .5s;
	}
</style>
