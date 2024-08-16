<template>
	<div class="footer-component">
		<div class="footer-component-links">
			<a href="/site/help">Help</a>
			<div class="spacer">·</div>
			<a href="/site/terms">Terms</a>
			<div class="spacer">·</div>
			<a href="/site/privacy">Privacy</a>
			<div class="spacer">·</div>
		</div>

		<div class="footer-component-attribution">
			<div><span>© {{ getYear() }} {{config.domain}}</span></div>
			<div class="spacer">·</div>
			<div><a href="https://krybot.com" class="text-bluegray-500 font-weight-bold">Powered by Krybot</a></div>
		</div>
	</div>
</template>

<script type="text/javascript">
	export default {
		data() {
			return {
				config: window.pfl
			}
		},

		methods: {
			getYear() {
				return (new Date().getFullYear());
			}
		}
	}
</script>
