<script context="module">
	export async function load({ page, fetch, session, context }) {
		// Sleep for 2 seconds
		const sleep = new Promise((resolve) => setTimeout(resolve, 2000));
		await sleep;
    // Have to return something properly finish this function
    // Typically you'll return props, errors, redirects etc
		return {};
	}
</script>

<div class="container">
	<div class="content">
		<h1>You're on Page 1.</h1>
		<p>
			In this page's <code>load</code> function, we waited for two seconds to mimick a real-world API
			call before rendering. You can go back to the home page, which should load instantaneously because
			it doesn't do much server side. Page 2, however, will have a longer delay of 5 seconds.
		</p>
		<div class="links">
			<a href="/">Home</a>
			<a href="/page-2">Page 2</a>
		</div>
	</div>
</div>
