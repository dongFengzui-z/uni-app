<template>
	<view class="container">
		<view class="title">
			<ul v-for="item in dataList">
				<li @click="tagTitle(item.title)">{{ item.title }}</li>
			</ul>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				dataList: [
					{title:"昨天"},{title:"今天"},{title:"明天"}
				]
			}
		},
		methods: {
			tagTitle(val) {
				console.log(val)
			}
		}
	}
</script>

<style scoped lang="scss">
	.container {
		padding: 20px;
		font-size: 14px;
		.title {
			ul {
				list-style: none;
				float: left;
				
			}
		}
	}
	
</style>
