<script lang="ts">
	import 'carbon-components-svelte/css/g90.css';
	import { MultiSelect } from 'carbon-components-svelte';
</script>

<main>
	<p>
		If <code>selectionFeedback</code> is set to <code>top-after-reopen</code> (default), selected
		items should be moved to the top after making the selection, closing and then re-opening the
		dropdown (<a
			target="_blank"
			href="https://react.carbondesignsystem.com/?path=/story/components-multiselect--default"
			>React reference</a
		>).
	</p>
	<hr />
	<MultiSelect
		titleText="Contact"
		label="Select contact methods..."
		items={[
			{ id: '0', text: 'Slack' },
			{ id: '1', text: 'Email' },
			{ id: '2', text: 'Fax' }
		]}
		selectionFeedback="top-after-reopen"
	/>
</main>

<style>
	:global(body) {
		display: flex;
		justify-content: center;
	}
	main {
		padding: 2rem;
		align-self: center;
		width: 100%;
		max-width: 900px;
	}
</style>
