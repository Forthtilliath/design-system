<script>
	import { theme } from './theme';
</script>

<div class="wrapper">
	<fieldset>
		<legend>Colors</legend>
		<label>
			Primary
			<input type="color" bind:value={$theme.color.primary} />
		</label>

		<label>
			Secondary
			<input type="color" bind:value={$theme.color.secondary} />
		</label>

		<label>
			Accent
			<input type="color" bind:value={$theme.color.accent} />
		</label>
	</fieldset>
	<fieldset>
		<legend>Fonts</legend>
		<label>
			Headers
			<input type="text" bind:value={$theme.font.header} />
		</label>
		<label>
			Base text
			<input type="text" bind:value={$theme.font.baseText} />
		</label>
	</fieldset>
</div>

<style>
	.wrapper {
		position: fixed;
		bottom: 0;
		right: 0;

		background: #f2f2f2;
			color: #1d1e22;

		@media (prefers-color-scheme: dark) {
			background: #1d1e22;
			color: #f2f2f2;
		}
	}
</style>
