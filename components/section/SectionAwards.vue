<template>
	<div class="awards">
		<div class="awards__title_cta">
			<div>
				<h2>Don’t just take our word for it</h2>
				<p>Internationally awarded for excellence</p>
			</div>

			<BaseCTAButton :text="'Open Trading Account'" />
		</div>
		<div class="awards__list">
			<NuxtImg v-for="(award, index) in awards" :key="index" :src="`/images/awards/${award}.svg`" class="awards__list_logo" alt="Award image" />
		</div>
		<div class="awards__cta_box">
			<h2>Take the next step and reserve your spot today</h2>
			<BaseCTAButton :text="'Reserve your spot now'" />
		</div>
	</div>
</template>

<script setup>
	const awards = [
		'pan-finance',
		'gbm',
		'gbm',
		'atoz',
		'world-finance'
	]
</script>