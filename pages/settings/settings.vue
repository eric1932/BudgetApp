<template>
	<view class = "settingsContents">
		<a href = "#/pages/settings/language/language" class = "settingItems">
		<view class = "str">
			语言
		</view> 
		</a><hr>
		<a href = "#/pages/settings/feedBack/feedBack" class = "settingItems">
		<view class = "str">
			建议反馈
		</view> 
		</a> 
		<hr>
		<a href = "#/pages/settings/reminder/reminder" class = "settingItems">
		<view class = "str">
			每月交易提醒
		</view>
		</a><hr>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
			}
		},
		methods: {
			test(){
				this.$router.go(-1)
			}
		}
	}
</script>

<style>
	a:link {
		color: black;
		text-decoration: none;
	},
	a:visited {
		color: black;
		text-decoration: none;
	}
	.settingItems {
		
	},
	.str {
		padding: 10px;
		background-color: aquamarine;
	
	}

</style>
