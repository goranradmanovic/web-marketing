<template>
	<footer class="footer">
		<div class="footer__contact">
			<div class="footer__contact_logo_copy">
				<BaseLogo :imgName="'dark'" />
				<p>&copy; SquaredFinancial 2025. All rights reserved.</p>
			</div>
			<div class="footer__contact_socials">
				<span>Find us on</span>
				<NuxtLink to="#" v-for="(icon, index) in socialIcons" :key="index">
					<NuxtImg :src="`/images/social/${icon}.svg`" class="about__media_companies_logo" alt="Company image" />
				</NuxtLink>
			</div>
			<div class="footer__contact_address">
				<h3>6B Adeniyi Jones Ikeja, Lagos, Nigeria</h3>
				<button>Contact us</button>
			</div>
		</div>

		<div class="footer__info">
			<div class="footer__info_risk">
				<h3>Risk warning:</h3>
				<p>Trading leveraged products involve a significant risk and can result in the loss of your invested capital.</p>
			</div>
			<div class="footer__info_disclaimers">
				<h3>Disclaimers:</h3>
				<p>The website is not intended to offering investment services to citizens of certain jurisdictions such as EU/EEA member states, UK, USA, Canada, Australia, New Zealand, FATF-listed countries including, among others, Iran, North Korea, and Myanmar (Burma). You must be 18 years old, or of legal age as determined in your country in order to register for an account.</p>
			</div>
			<div class="footer__info_legal">
				<h3>Legal:</h3>
				<p>This website is operated by SQ Sey Ltd, a company authorised and regulated as a Securities Dealer by the Financial Services Authority of Seychelles with license number SD024. SQ Sey Ltd is part of the ‘SquaredFinancial’ group of companies which includes Squared Financial (CY) Limited, a Cyprus company authorised and regulated by Cyprus Securities and Exchange Commission with license number 329/17.</p>
			</div>
		</div>
	</footer>
</template>

<script setup>
	const socialIcons = ['fb', 'x', 'ln', 'ig', 'tg', 'yt']
</script>