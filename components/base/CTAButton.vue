<template>
	<button class="cta">{{ text }}</button>
</template>

<script setup>
	const props = defineProps({
		text: {
			type: String,
			required: false,
			default: 'Subscribe for our free webinar'
		}
	})
</script>