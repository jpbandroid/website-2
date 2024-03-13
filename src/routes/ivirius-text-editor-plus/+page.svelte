<script>
  //Imports
	import * as Fluent from "fluent-svelte";
	import "fluent-svelte/theme.css";

  //Variables
  let open = true;
</script>

<!--Head-->
<svelte:head>
	<title>UltraTextEdit UWP Plus</title>
	<meta name="description" content="Professional text editor app for Windows 11" />
</svelte:head>

<section style="display: flex; flex-wrap: wrap; align-items: center; justify-content: flex-start; padding: 10px; background: rgba(25, 25, 25, 0.15); border-bottom: 1px solid rgba(205, 205, 205, 0.25);">
	<Fluent.PersonPicture src="https://yt3.googleusercontent.com/82KcuEjHraSZUui5_XY4uQj0uUgtcFr1G2DKlpGXyPIlJqd8uAunQqM5mG95sXdTbfqSqL1Npw=s176-c-k-c0x00ffffff-no-rj" style="width: 35px; height: 35px; margin-right: 15px; margin-left: 15px; margin-top: 18px; align-items: center;"/>

	<Fluent.Button style="height: 32px; margin-right: 15px; align-items: center;">Home</Fluent.Button>
	<Fluent.Button style="height: 32px; margin-right: 15px; align-items: center;" variant="hyperlink" onclick="window.location.href='https://errortek.vercel.app/crimsonui';">CrimsonUI</Fluent.Button>
	<Fluent.Button style="height: 32px; margin-right: 15px; align-items: center;" variant="hyperlink" onclick="window.location.href='https://errortek.vercel.app/documentations';">Documentations</Fluent.Button>
	<Fluent.Button style="height: 32px; margin-right: 15px; align-items: center;" variant="hyperlink" onclick="window.location.href='https://errortek.vercel.app/news';">News/Blog</Fluent.Button>
	<Fluent.Button style="height: 32px; margin-right: 15px; align-items: center;" variant="hyperlink" onclick="window.location.href='https://errortek.vercel.app/contact';">Contact</Fluent.Button>
	<Fluent.Button style="height: 32px; margin-right: 15px; align-items: center;" variant="hyperlink" onclick="window.location.href='https://errortek.vercel.app/about';">About</Fluent.Button>
</section>

<!--Title-->
<section class="centered-section">
	<h1>
		<Fluent.TextBlock variant="titleLarge">UltraTextEdit UWP Plus</Fluent.TextBlock>
	</h1>
 <h2>
		<Fluent.TextBlock variant="body" align="center">UTE UWP Plus is the next generation of modern text editing software on Windows!</Fluent.TextBlock>
 </h2>
</section>

<!--Download buttons-->
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

<!--Ivirius Hub-->
<section class="margin-section">
        <h1>
                <Fluent.TextBlock variant="subtitle">Ivirius Hub</Fluent.TextBlock>
        </h1>
        <h2>
                <Fluent.TextBlock variant="body">The Ivirius Hub is the sample app from Ivirius, offering the Ivirius.Windowing API for UWP child windows and CrimsonUI XAML code. Experience a fast and fluid sample app that showcases the capabilities of our well built tools. This versatile UWP and Windows App SDK hub is available for download on the Microsoft Store.</Fluent.TextBlock>
        </h2>
        <h3>
          <Fluent.Button variant="hyperlink" onclick="window.location.href='https://ivirius.vercel.app/ivirius-hub';">Learn more</Fluent.Button>
        </h3>
</section>

<!--CrimsonUI-->
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

<!--Bottom bar-->
<section style="padding-top: 10px; padding-bottom: 10px; padding-left: 25px; background: var(--fds-solid-background-base); border-top: 1px solid rgba(205, 205, 205, 0.25); display: flex; flex-direction: column; align-items: flex-start;">
	<Fluent.TextBlock variant="bodyStrong" style="margin-top: 10px;">
		Partners
	</Fluent.TextBlock>
	<Fluent.Button variant="hyperlink" onclick="window.location.href='https://ivirius.vercel.app';" style="margin-top: 10px; margin-bottom: 10px;">Ivirius</Fluent.Button>
	<Fluent.TextBlock variant="bodyStrong" style="margin-top: 10px;">
		Developers and contributors
	</Fluent.TextBlock>
	<Fluent.Button variant="hyperlink" onclick="window.location.href='https://ivirius.vercel.app/';" style="margin-top: 10px; margin-bottom: 10px;">Ivirius</Fluent.Button>
	<Fluent.TextBlock variant="bodyStrong" style="margin-top: 10px;">
		Website
	</Fluent.TextBlock>
	<Fluent.Button variant="hyperlink" onclick="window.location.href='https://fluent-svelte.vercel.app';" style="margin-top: 10px; margin-bottom: 10px;">Fluent Svelte</Fluent.Button>
	<Fluent.Button variant="hyperlink" onclick="window.location.href='https://www.vercel.com';">Vercel</Fluent.Button>
	<Fluent.Button variant="hyperlink" onclick="window.location.href='https://errortek.vercel.app/about';" style="margin-top: 10px; margin-bottom: 10px;">About</Fluent.Button>
</section>

<!--Styles-->
<style>
  /*Import theme*/
	@import url("https://unpkg.com/fluent-svelte/theme.css");

	/* Some base styles to get things looking right. */
	:global(body) 
  {
    /*Background color*/
		background-color: var(--fds-solid-background-base);

    /*Background image*/
    background-image: url("https://cdn.discordapp.com/attachments/1141503151808184401/1210350581504278618/1000030651-safeimagekit.jpeg.png?ex=65ea3dd1&is=65d7c8d1&hm=facb30449de806bcb7bb777bd14e81dddb7bf7de9e882144896e0bc80b304153&");
    
    /*Background color*/
		color: var(--fds-text-primary);
	}

  /*Centered section*/
  .centered-section 
  {
    text-align: center;
    margin: 0 auto;
    padding: 25px;
  }

  /*Left aligned centered section*/
  .margin-section 
  {
    margin: 0 auto;
    padding: 25px;
  }
</style>