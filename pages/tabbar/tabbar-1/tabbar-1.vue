<template>
	<view class="content">
		页面 - 1
		<uni-badge text="1"></uni-badge>
		<uni-badge text="3" type="primary" :inverted="true"></uni-badge>
		<view class="">
			<u-action-sheet :list="list" v-model="show"></u-action-sheet>
		</view>
	</view>
</template>

<script>
export default {
	data() {
		return {
			title: 'Hello',
			list: [{
				text: '点赞',
				color: 'blue',
				fontSize: 28
			}, {
				text: '分享'
			}, {
				text: '评论'
			}],
			show: true
		};
	},
	onLoad() {},
	methods: {}
};
</script>

<style>
.content {
	text-align: center;
	height: 400upx;
	margin-top: 200upx;
}
</style>
