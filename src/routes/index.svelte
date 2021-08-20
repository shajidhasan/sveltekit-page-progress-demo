<div class="container">
	<div class="content">
		<h1>Page loading progress bar in action with SvelteKit.</h1>
		<p>
			Click a link below to go to some other page. SvelteKit has a <code>load</code> function which runs in the server to load data through API calls. To mimick a real-world use of the <code>load</code> function, we'll run an empty <code>setTimeout</code> in a <code>Promise</code> to wait for 2 seconds.
		</p>
		<div class="links">
			<a href="/page-1">Page 1</a>
			<a href="/page-2">Page 2</a>
		</div>
	</div>
</div>
