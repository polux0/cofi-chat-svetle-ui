<script>
	// Define a fixed name variable (private to the component)
	let name = "Minimalist Cofi.chat(bot)";
</script>

<main>
	<h1>{name}</h1>
	<iframe id="streamlit"
		src="https://minimalist-cofi-chat.streamlit.app//?embed=true&embed_options=light_theme"
		title = "Minimalist cofi.chat(bot)"
		height="450"
		style="width:100%;border:none;">
	</iframe>
</main>

<!-- Technical debt -->
<!-- 1. We should resolve issues with 640px mobile screen sizes:
	 	- heading is not centered 
	 	- streamlit app is not wide enough
-->
<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}
	iframe {
		height: 900px;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}
	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>