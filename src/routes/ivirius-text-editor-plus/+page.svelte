<script>
	import * as Fluent from "fluent-svelte";
	import "fluent-svelte/theme.css";
</script>

<svelte:head>
	<title>UltraTextEdit UWP Plus</title>
	<meta name="description" content="Professional text editor app for Windows 11" />
</svelte:head>

<section class="centered-section">
	<h1>
		<Fluent.TextBlock variant="titleLarge">UltraTextEdit UWP Plus</Fluent.TextBlock>
	</h1>
 <h2>
		<Fluent.TextBlock variant="body" align="center">UTE UWP Plus is the next generation of modern text editing software on Windows!</Fluent.TextBlock>
 </h2>
</section>
 
<section class="centered-section">
	<h2>
		<Fluent.Button variant="accent" onclick="window.location.href='';">Download (coming soon)</Fluent.Button>
		<Fluent.Button variant="hyperlink" style="margin: 15px" onclick="window.location.href='https://github.com/jpbandroid/UTE-UWP-Plus';">GitHub</Fluent.Button>
	</h2>
</section>
 
<section class="margin-section">
	<h1>
		<Fluent.TextBlock variant="subtitle">Feature-complete</Fluent.TextBlock>
 </h1>
 <h2>
		<Fluent.TextBlock variant="body">UTE UWP Plus has all the features you would expect from a text editor, as well as some extra features and customisation options.</Fluent.TextBlock>
	</h2>

</section>
 
<section class="margin-section">
	<h1>
		<Fluent.TextBlock variant="subtitle">Modern design</Fluent.TextBlock>
 </h1>
 <h2>
		<Fluent.TextBlock variant="body">UTE UWP Plus uses the latest version of WinUI (and will add an option to use </Fluent.TextBlock>
<Fluent.Button style="padding: 0px" variant="hyperlink"  onclick="window.location.href='https://errortek.vercel.app/crimsonui';">CrimsonUI</Fluent.Button>
<Fluent.TextBlock variant="body"> in the future) for the main layout, making it consistent with the Windows 11 design.</Fluent.TextBlock>
	</h2>
</section>

<style>
	@import url("https://unpkg.com/fluent-svelte/theme.css");

	/* Some base styles to get things looking right. */
	:global(body) {
		background-color: var(--fds-solid-background-base);
		color: var(--fds-text-primary);
	}
    .centered-section {
        text-align: center;
    }
    .margin-section {
        margin: 25px;
    }
</style>