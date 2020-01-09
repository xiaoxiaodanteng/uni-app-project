<template>
	<view>
		
		<!-- tabs -->
		<view class="tui-mtop">
			<tui-tabs :tabs="tabs" :currentTab="currentTab>2?0:currentTab" @change="change" itemWidth="33.3333%"></tui-tabs>
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
			change(e) {
				this.currentTab = e.index
			},
		}
	}
</script>

<style>

</style>
