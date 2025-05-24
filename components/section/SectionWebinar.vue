<template>
	<section class="webinar">
		<div class="webinar__cards">
			<div v-for="(webinar, index) in webinars" :key="index" class="webinar__card">
				<h2>{{ webinar.title }}</h2>
				<ul class="webinar__card_list">
					<li v-for="(item) in webinar.lists" :key="index">{{ item }}</li>
				</ul>
			</div>
		</div>

		<BaseCTAButton />
	</section>
</template>

<script setup>
	const webinars = [
		{
			title: 'Unlock your future self after this webinar',
			lists: [
				'Confident when approaching global markets.',
				'Disciplined when setting your trading plans.',
				'Strategic when seizing new market opportunities.',
				'Resilient when handling market volatility with strength and focus.'
			]
		},
		{
			title: 'Capitalize on this webinars and...',
			lists: [
				'Ask your questions to the host directly.',
				'Get answers on spot.',
				'Schedule a one-on-one session with the mentors.',
				'Interact with other participants.'
			]
		}
	]
</script>