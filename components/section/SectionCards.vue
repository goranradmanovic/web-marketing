<template>
	<section class="cards">
		<div class="cards_wrapper">
			<div v-for="(card, index) in cards" :key="index" class="card">
				<NuxtImg v-if="card.img" :src="`/images/${card.img}`" class="card__img" alt="Card icon" />
				<p v-html="card.text" class="card__text"></p>
			</div>
		</div>
	</section>
</template>

<script setup>
	const cards = [
		{
			text: 'Why Temitope is your ultimate mentor',
			img: ''
		},
		{
			text: 'SquaredFinancial’s Forex trading expert, <strong>Temitope Ijibadejo</strong>, uncovers new roads you can take to advance your trading skills. Join our trading webinar and unlock countless opportunities.',
			img: ''
		},
		{
			text: '<strong>He goes beyond regular analysis and uncovers deep insights that others miss</strong>',
			img: 'icons/loop.svg'
		},
		{
			text: '<strong>He breaks down complex economic trends and gives actionable strategies</strong>',
			img: 'icons/bar-chart.svg'
		},
		{
			text: '<strong>He is a trusted voice in the region and provides an in-depth outlook on top financial media</strong>',
			img: ''
		},
		{
			text: '<strong>He is focused on customized performance and results and empowers traders with efficient techniques</strong>',
			img: 'icons/line-chart.svg'
		},
		{
			text: '<strong>Take the next step and reserve your spot <br/> today</strong>',
			img: ''
		},
		{
			text: '',
			img: ''
		},
	]
</script>