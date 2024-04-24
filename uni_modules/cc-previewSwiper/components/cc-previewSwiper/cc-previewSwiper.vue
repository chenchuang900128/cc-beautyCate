<template>
	<view class="swiper">
		<swiper class="swiper-container" :autoplay="true" :interval="4000" :circular="true"
			:indicator-dots="true" indicator-active-color="#FF2638" indicator-color="#cccccc">
			<block v-for="(item, index) in goods.images" :key="item">
				<swiper-item class="swiper-wrapper">
					<image :src="item" mode="widthFix" class="is-response" lazy-load="true" :data-index="index"
						@tap="previewPhoto"></image>
				</swiper-item>
			</block>
		</swiper>
	</view>
</template>
<script>
</script>
<style>
</style>
