<script context="module">
	export async function load({ page, fetch, session, context }) {
		// Sleep for 5 seconds
		const sleep = new Promise((resolve) => setTimeout(resolve, 5000));
		await sleep;
    // Have to return something properly finish this function
    // Typically you'll return props, errors, redirects etc
		return {};
	}
</script>


<div class="container">
	<div class="content">
		<h1>You're on Page 2.</h1>
		<p>
			In this page's <code>load</code> function, we waited for <i>five seconds</i> to mimick a real-world
			API call before rendering. It's actually probably too long, but this is purely for demonstration
			purposes. You can go back to the home page, which should load instantaneously because it doesn't
			do much server side.
		</p>
		<div class="links">
			<a href="/">Home</a>
			<a href="/page-1">Page 1</a>
		</div>
	</div>
</div>
