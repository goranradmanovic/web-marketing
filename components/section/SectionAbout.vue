<template>
	<div class="about">
		<div class="about__title">
			<h2>About</h2>
			<BaseLogo :imgName="'dark'" />
		</div>
		<div class="about__schema">
			<div>
				<p>More than just a broker – A thriving community & learning hub</p>
				<h2>We help our traders thrive</h2>
			</div>
			<BaseCTAButton :text="'Open Trading Account'" />
		</div>
		<div class="about__media">
			<h2>Expertise and coverage by global media</h2>

			<div class="about__media_companies">
				<NuxtImg v-for="(company, index) in companies" :key="index" :src="`/images/companies/${company}.svg`" class="about__media_companies_logo" alt="Company image" />
			</div>
		</div>
	</div>
</template>


<script setup>
	const companies = [
		'cnbc',
		'bloomberg',
		'sky-news',
		'alarabiya',
		'asharq-news',
		'finance-magnates',
		'fxstreet'
	]
</script>