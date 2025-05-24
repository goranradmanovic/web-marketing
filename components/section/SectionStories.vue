<template>
	<div class="stories">
		<div class="stories__title_cta">
			<h2>Proven by trader success stories</h2>
			<BaseCTAButton :text="'Reserve your spot now'" />
		</div>
		<div class="stories__content">
			<div v-for="(story, index) in stories" :key="index" :class="{ box: story.boxLayout, rectangle: !story.boxLayout }" class="stories__content_card">
				<NuxtImg src="/images/icons/stars.svg" class="stories__content_card_img" alt="Stars icon" />
				<p>{{ story.text }}</p>
			</div>
		</div>
	</div>
</template>

<script setup>
	const stories = [
		{
			text : 'WebinarJam is an excellent webinar platform to host one-off and webinar series. It\'s simple to set up, reliable and does the job very well. My attendees love the experience and I find it a breeze to run multiple webinar series catering to 50 - 300+ people during the sessions.',
			boxLayout: true
		},
		{
			text : 'WebinarJam is an excellent webinar platform to host one-off and webinar series. It\'s simple to set up, reliable and does the job very well. My attendees love the experience and I find it a breeze to run multiple webinar series catering to 50 - 300+ people during the sessions.',
			boxLayout: true
		},
		{
			text : 'WebinarJam is an excellent webinar platform to host one-off and webinar series. It\'s simple to set up, reliable and does the job very well. My attendees love the experience and I find it a breeze to run multiple webinar series catering to 50 - 300+ people during the sessions.',
			boxLayout: true
		},
		{
			text : 'WebinarJam is an excellent webinar platform to host one-off and webinar series. It\'s simple to set up, reliable and does the job very well. My attendees love the experience and I find it a breeze to run multiple webinar series catering to 50 - 300+ people during the sessions.',
			boxLayout: false
		},
		{
			text : 'WebinarJam is an excellent webinar platform to host one-off and webinar series. It\'s simple to set up, reliable and does the job very well. My attendees love the experience and I find it a breeze to run multiple webinar series catering to 50 - 300+ people during the sessions.',
			boxLayout: false
		}

	]
</script>