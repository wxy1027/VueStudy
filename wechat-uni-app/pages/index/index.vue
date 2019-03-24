<template>
	<view class="content">
		
			<view class="item" v-for="(row,index) in rows" :key="index">
				<image :src="row.avatar" id="row-avatar"></image>
				<view class="row-center">
					<view class="row-name">
						<text>{{row.name}}</text>
						<text class="row-time">{{row.time}}</text>
					</view>
					<navigator url="messages" hover-class="navigator-hover" class="nav">
					<text class="row-message">{{row.message}}</text>
					</navigator>
				</view>
			</view>
		
		
	</view>
</template>

<script>
	export default {
		data() {
			return {
				rows: [{
						avatar: '../../static/avatar1.jpg',
						name: '孙鸣',
						message: '我通过了你的朋友验证请求，现在我',
						time: '09:36'
					},
					{
						avatar: '../../static/avatar2.jpg',
						name: 'thfy10yf',
						message: '好的',
						time: '08:55'
					},
					{
						avatar: '../../static/avatar3.jpg',
						name: '刘飞',
						message: '帮帮忙公司要求一个人18个名额，可抵一个工时',
						time: '07:35'
					},
					{
						avatar: '../../static/avatar4.jpg',
						name: '郭教练',
						message: '我有优惠政策来找我',
						time: '09:36'
					},
					{
						avatar: '../../static/avatar5.jpg',
						name: '妈妈',
						message: '在不在',
						time: '昨天'
					},
					{
						avatar: '../../static/avatar6.jpg',
						name: '辛玲',
						message: '嗯嗯',
						time: '周一'
					},
					{
						avatar: '../../static/avatar1.jpg',
						name: '素质拓展',
						message: '心田荷叶：那就好',
						time: '周一'
					},
					{
						avatar: '../../static/avatar3.jpg',
						name: '蔡建',
						message: '嗯呢',
						time: '3月17日'
					},
					{
						avatar: '../../static/avatar5.jpg',
						name: '郭志豪',
						message: '好的，谢谢啦~',
						time: '3月15日'
					},
				],
			}
		},
		onLoad() {

		},
		methods: {
		}
	}
</script>

<style>
	.title {
		font-size: 36upx;
		color: #8f8f94;
	}
	.item {
		height: 150upx;
		display: flex;
		margin-top: 10upx;
	}
	#row-avatar {
		width: 130upx;
		height: 130upx;
		margin-left: 10upx;
		margin-top: 15upx;
	}
	.row-center {
		flex: 1 1 40%;
		display: flex;
		flex-direction: column;
		border-bottom: 1upx solid #EEEEEE;
		margin-left: 40upx;
		margin-top: 30upx;
	}
	.row-name {
		display: flex;
		justify-content: space-between;
		margin-top: 10upx;
		font-size: 35upx;
	}
	.row-time {
		color: #8F8F94;
		font-size: 25upx;
		margin-right: 25upx;
	}
	.row-message {
		color: #8F8F94;
		font-size: 25upx;
		margin-top: 25upx;
	}
	.nav{
		margin-top: 10upx;
	}
</style>
