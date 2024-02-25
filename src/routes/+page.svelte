<script>
  //Imports
	import * as Fluent from "fluent-svelte";
	import "fluent-svelte/theme.css";

  //Variables
  let open = true;
</script>

<!--Head-->
<svelte:head>
	<title>ErrorTek's Website</title>
	<meta name="description" content="Ivirius official website"/>
</svelte:head>
  
<section style="display: flex; flex-wrap: wrap; align-items: center; justify-content: flex-start; padding: 10px; background: rgba(25, 25, 25, 0.15); border-bottom: 1px solid rgba(205, 205, 205, 0.25);">
  <Fluent.PersonPicture src="https://yt3.googleusercontent.com/82KcuEjHraSZUui5_XY4uQj0uUgtcFr1G2DKlpGXyPIlJqd8uAunQqM5mG95sXdTbfqSqL1Npw=s176-c-k-c0x00ffffff-no-rj" style="width: 35px; height: 35px; margin-right: 15px; margin-left: 15px; margin-top: 18px; align-items: center;"/>

  <Fluent.Button style="height: 32px; margin-right: 15px; align-items: center;">Home</Fluent.Button>
  <Fluent.Button style="height: 32px; margin-right: 15px; align-items: center;" variant="hyperlink" onclick="window.location.href='https://errortek.vercel.app/crimsonui';">CrimsonUI</Fluent.Button>
  <Fluent.Button style="height: 32px; margin-right: 15px; align-items: center;" variant="hyperlink" onclick="window.location.href='https://errortek.vercel.app/documentations';">Documentations</Fluent.Button>
  <Fluent.Button style="height: 32px; margin-right: 15px; align-items: center;" variant="hyperlink" onclick="window.location.href='https://errortek.vercel.app/contact';">Contact</Fluent.Button>
  <Fluent.Button style="height: 32px; margin-right: 15px; align-items: center;" variant="hyperlink" onclick="window.location.href='https://errortek.vercel.app/about';">About</Fluent.Button>
</section>

<!--Title-->
<section class="centered-section">
	<h1>
		<Fluent.TextBlock variant="titleLarge"></Fluent.TextBlock>
	</h1>
 <h2>
		<Fluent.TextBlock variant="body" align="center">Welcome to my website! I'm just an average tech YouTuber with 148 subscribers, as well as the developer of a few projects, including UTE UWP, WIndivs, jpbROM and many others, as well as co-developing Ivirius Text Editor, Ivirius Hub and the CrimsonUI UI library!</Fluent.TextBlock>
 </h2>
</section>

<!--Download buttons-->
<section class="centered-section">
	<h2>
		<Fluent.Button variant="accent" onclick="window.location.href='';">Download UTE UWP Plus</Fluent.Button>
		<Fluent.Button style="margin: 15px">Download UTE UWP</Fluent.Button>
		<Fluent.Button>Download Ivirius Hub (CrimsonUI demo app)</Fluent.Button>
	</h2>
</section>

<!--InfoBar-->
 <section class="margin-section">
	<h2>
		<Fluent.InfoBar severity="caution" title="Important!" message="This is the only finished page of this website. The rest are actively being worked on. Thank you for your patience." style="max-width:550px;"/>
	</h2>
</section>

<!--Ivirius Text Editor Plus-->
<section class="margin-section">
        <h1>
                <Fluent.TextBlock variant="subtitle">UltraTextEdit UWP+</Fluent.TextBlock>
        </h1>
        <h2>
                <Fluent.TextBlock variant="body">UTE UWP Plus is the next generation of modern text editing software on Windows! Major features include compliance to the latest Fluent Design guidelines and best practices as well as always using an up-to-date version of WinUI.</Fluent.TextBlock>
        </h2>
        <h3>
          <Fluent.Button variant="hyperlink" onclick="window.location.href='https://errortek.vercel.app/ivirius-text-editor-plus';">Learn more</Fluent.Button>
        </h3>
</section>

<section class="margin-section">
        <h1>
                <Fluent.TextBlock variant="subtitle">UltraTextEdit UWP</Fluent.TextBlock>
        </h1>
        <h2>
                <Fluent.TextBlock variant="body">UTE UWP is a modern text editor with the Fluent Design guidelines in mind for all your text editing needs! Plus, it gets preview updates via a preview system and monthly updates with bug fixes and library updates every month!</Fluent.TextBlock>
        </h2>
        <h3>
          <Fluent.Button variant="hyperlink" onclick="window.location.href='';">Learn more (coming soon)</Fluent.Button>
        </h3>
</section>

<!--CrimsonUI-->
<section class="margin-section">
        <h1>
                <Fluent.TextBlock variant="subtitle">CrimsonUI</Fluent.TextBlock>
        </h1>
        <h2>
                <Fluent.TextBlock variant="body">CrimsonUI is a dynamic UI library designed for UWP and Windows App SDK. Rooted in WinUI and influenced by FireCube's GlowUI, CrimsonUI seamlessly blends default WinUI elements with glowing, shiny components. Immerse yourself in stunning animations, ensuring a very smooth and beautiful user experience. Elevate your app's visual appeal with the elegance of CrimsonUI.</Fluent.TextBlock>
        </h2>
        <h3>
          <Fluent.Button variant="hyperlink" onclick="window.location.href='https://errortek.vercel.app/crimsonui';">Learn more</Fluent.Button>
        </h3>
</section>

<!--Bottom bar-->
<section style="padding-top: 10px; padding-bottom: 10px; padding-left: 25px; background: var(--fds-solid-background-base); border-top: 1px solid rgba(205, 205, 205, 0.25); display: flex; flex-direction: column; align-items: flex-start;">
  <Fluent.TextBlock variant="bodyStrong" style="margin-top: 10px;">
    Partners
  </Fluent.TextBlock>
          <Fluent.Button variant="hyperlink" onclick="window.location.href='https://www.spoo.me';" style="margin-top: 10px; margin-bottom: 10px;">spoo.me URL shortener</Fluent.Button>
  <Fluent.TextBlock variant="bodyStrong" style="margin-top: 10px;">
    Developers and contributors
  </Fluent.TextBlock>
          <Fluent.Button variant="hyperlink" onclick="window.location.href='https://website-2-sigma.vercel.app/';" style="margin-top: 10px; margin-bottom: 10px;">ErrorTek</Fluent.Button>
  <Fluent.TextBlock variant="bodyStrong" style="margin-top: 10px;">
    Website
  </Fluent.TextBlock>
          <Fluent.Button variant="hyperlink" onclick="window.location.href='https://fluent-svelte.vercel.app';" style="margin-top: 10px; margin-bottom: 10px;">Fluent Svelte</Fluent.Button>
          <Fluent.Button variant="hyperlink" onclick="window.location.href='https://www.vercel.com';">Vercel</Fluent.Button>
          <Fluent.Button variant="hyperlink" onclick="window.location.href='https://ivirius.vercel.app/about';" style="margin-top: 10px; margin-bottom: 10px;">About</Fluent.Button>
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
    max-width: 1250px;
  }

  /*Left aligned centered section*/
  .margin-section 
  {
    margin: 0 auto;
    padding: 25px;
    max-width: 1250px;
  }
</style>