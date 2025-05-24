<template>
	<NuxtImg :src="`/images/logo/${imgName}.svg`" class="logo" alt="Logo image" />
</template>

<script setup>
	const props = defineProps({
		imgName: {
			type: String,
			required: false,
			default: 'light'
		}
	})
</script>