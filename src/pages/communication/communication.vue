<template>
	<view>
		
		<!-- tabs -->
		<view>
			<tui-tabs
				:tabs="tabs"
				bg-color="#ffffff"
			></tui-tabs>
		</view>
	</view>
</template>

<script>
	import tuiTabs from '@/components/tui-tabs/tui-tabs.vue'
	export default {
		components: {
			tuiTabs
		},
		data() {
			return {
				currentTab: 0,
				tabs: [
					{
						name: '交流'
					},
					{
						name: '任务'
					},
					{
						name: '组织'
					}
				]
			}
		},
		methods: {
			
		}
	}
</script>

<style>

</style>
