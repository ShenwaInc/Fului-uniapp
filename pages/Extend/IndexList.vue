<template>
	<view class="">
		<FuiNavBar class="bg-blue">
			<block slot="title">文本</block>
		</FuiNavBar>
		<view class="indexs">

			<view class="padding-tb-sm">
				<input class="fui-input--search " type="text" placeholder="搜索" confirm-type="search">
				</input>
			</view>
			<scroll-view scroll-y class="indexes" :scroll-into-view="'indexes-'+ listCurID"
				style="height:calc(100vh - 290rpx)" :scroll-with-animation="true" :enable-back-to-top="true">
				<block v-for="(item,index) in list" :key="index">
					<view :class="'indexItem-' + item.name" :id="'indexes-' + item.name" :data-index="item.name">
						<view class="padding-xs text-grey">{{item.name}}</view>
						<view class="card ">
							<view class="card-item" v-for="(items,sub) in 4" :key="sub">
								<view class="content padding-sm line-b">
									<view class="">江泽民</view>
									<view class="text-grey font-lg">1888888888
									</view>
								</view>
							</view>
						</view>
					</view>
				</block>
			</scroll-view>
			<view class="indexBar" style="height:calc(100vh - 290rpx)">
				<view class="indexBar-box" @touchstart="tStart" @touchend="tEnd" @touchmove.stop="tMove">
					<view class="indexBar-item" v-for="(item,index) in list" :key="index" :id="index"
						@touchstart="getCur" @touchend="setCur"> {{item.name}}</view>
				</view>
			</view>
			<!--选择显示-->
			<view v-show="!hidden" class="indexToast">
				{{listCur}}
			</view>
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
				hidden: true,
				listCurID: '',
				list: [],
				listCur: '',
			};
		},
		onLoad() {
			let list = [{}];
			for (let i = 0; i < 26; i++) {
				list[i] = {};
				list[i].name = String.fromCharCode(65 + i);
			}
			this.list = list;
			this.listCur = list[0];
			console.log(this.list)
		},
		onReady() {
			let that = this;
			uni.createSelectorQuery().select('.indexBar-box').boundingClientRect(function(res) {
				that.boxTop = res.top
			}).exec();
			uni.createSelectorQuery().select('.indexes').boundingClientRect(function(res) {
				that.barTop = res.top
			}).exec()
		},
		methods: {
			//获取文字信息
			getCur(e) {
				this.hidden = false;
				this.listCur = this.list[e.target.id].name;
			},
			setCur(e) {
				this.hidden = true;
				this.listCur = this.listCur
			},
			//滑动选择Item
			tMove(e) {
				let y = e.touches[0].clientY,
					offsettop = this.boxTop,
					that = this;
				//判断选择区域,只有在选择区才会生效
				if (y > offsettop) {
					let num = parseInt((y - offsettop) / 20);
					this.listCur = that.list[num].name
				};
			},

			//触发全部开始选择
			tStart() {
				this.hidden = false
			},

			//触发结束选择
			tEnd() {
				this.hidden = true;
				this.listCurID = this.listCur
			},
			indexSelect(e) {
				let that = this;
				let barHeight = this.barHeight;
				let list = this.list;
				let scrollY = Math.ceil(list.length * e.detail.y / barHeight);
				for (let i = 0; i < list.length; i++) {
					if (scrollY < i + 1) {
						that.listCur = list[i].name;
						that.movableY = i * 20
						return false
					}
				}
			}
		}
	}
</script>

<style scoped>
	.fui-input--search {
		background-color: #FFFFFF;
		border-radius: 10rpx;
		width: 720rpx;
		height: 70rpx;
		margin: 0 auto;
	}

	.indexes {
		position: relative;

	}

	.indexBar {
		position: fixed;
		right: 0px;
		bottom: 0px;
		padding: 20upx 20upx 20upx 60upx;
		display: flex;
		align-items: center;
	}

	.indexBar .indexBar-box {
		width: 40upx;
		height: auto;
		/* background: #fff; */
		background-color: transparent;
		display: flex;
		flex-direction: column;
		/* box-shadow: 0 0 20upx rgba(0, 0, 0, 0.1); */
		border-radius: 10upx;
	}

	.indexBar-item {
		flex: 1;
		width: 40upx;
		height: 40upx;
		display: flex;
		align-items: center;
		justify-content: center;
		font-size: 24upx;
		color: #2C5EC2;

	}

	movable-view.indexBar-item {
		width: 40upx;
		height: 40upx;
		z-index: 9;
		position: relative;
	}

	movable-view.indexBar-item::before {
		content: "";
		display: block;
		position: absolute;
		left: 0;
		top: 10upx;
		height: 20upx;
		width: 4upx;
		background-color: #f37b1d;
	}

	.indexToast {
		position: fixed;
		top: 0;
		right: 80upx;
		bottom: 0;
		background: rgba(0, 0, 0, 0.5);
		width: 100upx;
		height: 100upx;
		border-radius: 10upx;
		margin: auto;
		color: #fff;
		line-height: 100upx;
		text-align: center;
		font-size: 48upx;
	}

	.card {
		background-color: #FFFFFF;
	}

	.card-item .content {}
</style>
