<template>
	<view style="flex-direction: column;">
		<label id="summary">
			<text id="summary-prompt">今日开支</text>
			<text id="summary-value">$0.00</text>
		</label>
		
		<label>Filter TODO</label>
		
		<view>
			<view class="uni-title uni-common-mt">
				Vertical Scroll
				<text>\n纵向滚动</text>
			</view>
			<view>
				<scroll-view :scroll-top="scrollTop" scroll-y="true" class="scroll-Y" @scrolltoupper="upper" @scrolltolower="lower"
				@scroll="scroll">
					<HomeItem></HomeItem>
					<HomeItem></HomeItem>
					<HomeItem></HomeItem>
					
					<view id="demo1" class="scroll-view-item uni-bg-red">A</view>
					<view id="demo2" class="scroll-view-item uni-bg-green">B</view>
					<view id="demo3" class="scroll-view-item uni-bg-blue">C</view>
				</scroll-view>
			</view>
			<view @tap="goTop" class="uni-link uni-center uni-common-mt">
				点击这里返回顶部
			</view>
		</view>
	</view>
</template>

<script>
	import HomeItem from '../../components/HomeItem.vue';
	
	export default {
		data() {
			return {
				
			}
		},
		methods: {
			
		},
		components: {
			HomeItem,
		}
	}
</script>

<style>
	#summary {
		background-color: #53C21D;
		
		display: flex;
		/* justify-content: center; */
		height: 200rpx;
		
		margin: 25rpx;
		border-radius: 15px;
	}
	
	#summary-prompt {
		color: white;
		
		font-family: sans-serif;
		font-size: 32rpx;
		
		position: absolute;
		margin-left: 35rpx;
		margin-top: 35rpx;
	}
	
	#summary-value {
		color: white;
		
		font-family: sans-serif;
		font-size: 48rpx;
		
		position: absolute;
		margin-left: 35rpx;
		margin-top: 100rpx;
	}
	
	
	
	
	
	
	
	
	
	
	
	.scroll-Y {
		height: 300rpx;
	}
	
	.scroll-view_H {
		white-space: nowrap;
		width: 100%;
	}
	
	.scroll-view-item {
		height: 300rpx;
		line-height: 300rpx;
		text-align: center;
		font-size: 36rpx;
	}
	
	.scroll-view-item_H {
		display: inline-block;
		width: 100%;
		height: 300rpx;
		line-height: 300rpx;
		text-align: center;
		font-size: 36rpx;
	}
</style>
