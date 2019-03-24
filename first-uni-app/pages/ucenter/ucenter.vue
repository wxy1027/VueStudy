<template>
	<view class="content">
		<view>
			<text class="title">{{name}}</text>
			<!-- 超链接 -->
			<navigator url="setting" hover-class="navigator-hover">
				<button type="primary">个人设置</button>
			</navigator>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				name: '王欣雅'
			}
		},
		onLoad() {

		},
		methods: {

		}
	}
</script>

<style>
	.content {
		text-align: center;
		height: 400upx;
	}

	.title {
		font-size: 36upx;
		color: #8f8f94;
	}
</style>
