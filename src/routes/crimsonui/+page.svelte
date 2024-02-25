<script>
  //Imports
	import * as Fluent from "fluent-svelte";
  import "./styles.css";
  
  //Variables
  let open = true;
</script>

<!--Head-->
<svelte:head>
        <title>ErrorTek's Website</title>
        <meta name="description" content="ErrorTek's official website" />
</svelte:head>

<section style="display: flex; flex-wrap: wrap; align-items: center; justify-content: flex-start; padding: 10px; background: rgba(25, 25, 25, 0.15); border-bottom: 1px solid rgba(205, 205, 205, 0.25);">
  <Fluent.PersonPicture src="https://yt3.googleusercontent.com/82KcuEjHraSZUui5_XY4uQj0uUgtcFr1G2DKlpGXyPIlJqd8uAunQqM5mG95sXdTbfqSqL1Npw=s176-c-k-c0x00ffffff-no-rj" style="width: 35px; height: 35px; margin-right: 15px; margin-left: 15px; margin-top: 18px; align-items: center;"/>

  <Fluent.Button style="height: 32px; margin-right: 15px; align-items: center;" variant="hyperlink" onclick="window.location.href='https://errortek.vercel.app';">Home</Fluent.Button>
  <Fluent.Button style="height: 32px; margin-right: 15px; align-items: center;">CrimsonUI</Fluent.Button>
  <Fluent.Button style="height: 32px; margin-right: 15px; align-items: center;" variant="hyperlink" onclick="window.location.href='https://errortek.vercel.app/documentations';">Documentations</Fluent.Button>
  <Fluent.Button style="height: 32px; margin-right: 15px; align-items: center;" variant="hyperlink" onclick="window.location.href='https://errortek.vercel.app/contact';">Contact us</Fluent.Button>
  <Fluent.Button style="height: 32px; margin-right: 15px; align-items: center;" variant="hyperlink" onclick="window.location.href='https://errortek.vercel.app/about';">About</Fluent.Button>
</section>

<!--Title-->
<section class="centered-section">
	<h1>
		<Fluent.TextBlock variant="titleLarge">CrimsonUI</Fluent.TextBlock>
	</h1>
 <h2>
		<Fluent.TextBlock variant="body">Shiny, glowing UI elements.</Fluent.TextBlock>
 </h2>
</section>

<!--Download buttons-->
<section class="centered-section">
	<h2>
		<Fluent.Button variant="accent" onclick="window.location.href='https://apps.microsoft.com/detail/9N4T9H9182J5?hl=en-US';" disabled="true">Download CrimsonUI</Fluent.Button>
	</h2>
</section>

 <section class="margin-section">
	<h2>
		<Fluent.InfoBar severity="information" title="Description" message="CrimsonUI is a dynamic UI library designed for UWP and Windows App SDK. Rooted in WinUI and influenced by FireCube's GlowUI, CrimsonUI seamlessly blends default WinUI elements with glowing, shiny components. Immerse yourself in stunning animations, ensuring a very smooth and beautiful user experience. Elevate your app's visual appeal with the elegance of CrimsonUI." style="max-width:750px;"/>
	</h2>
 </section>

<section class="margin-section">
        <h1>
                <Fluent.TextBlock variant="subtitle">Easily blending in</Fluent.TextBlock>
        </h1>
        <h2>
                <Fluent.TextBlock variant="body">CrimsonUI controls are designed to integrate flawlessly with Windows applications, providing a seamless user interface experience. They feature rest brushes that are meticulously crafted to match the standard WinUI controls, ensuring a consistent and harmonious visual integration. This design philosophy allows for a cohesive user experience, where the CrimsonUI elements blend naturally with the native components of the Windows environment. The controls are built with attention to detail, aiming to enhance the aesthetics and functionality of applications while maintaining a familiar look and feel that users trust. With CrimsonUI, developers can elevate their application's interface, making it not only visually appealing but also intuitively usable, leveraging the robustness of Windows' native UI elements.</Fluent.TextBlock>
        </h2>
</section>

<section class="margin-section">
        <h1>
                <Fluent.TextBlock variant="subtitle">Simply beautiful</Fluent.TextBlock>
        </h1>
        <h2>
                <Fluent.TextBlock variant="body">CrimsonUI’s design leverages the visual appeal of glowing panels and accent color gradients to create a dynamic 3D appearance, reminiscent of a neon glow. This effect adds depth and a touch of modernity to the user interface, ensuring that applications not only function well but also stand out with a contemporary, eye-catching aesthetic. The use of gradients and light effects in CrimsonUI controls helps to bring interfaces to life, making them more engaging and visually stimulating for users.</Fluent.TextBlock>
        </h2>
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
        </h3>
</section>

<section class="margin-section">
        <h1>
                <Fluent.TextBlock variant="subtitle">CrimsonUI</Fluent.TextBlock>
        </h1>
        <h2>
                <Fluent.TextBlock variant="body">CrimsonUI is a dynamic UI library designed for UWP and Windows App SDK. Rooted in WinUI and influenced by FireCube's GlowUI, CrimsonUI seamlessly blends default WinUI elements with glowing, shiny components. Immerse yourself in stunning animations, ensuring a very smooth and beautiful user experience. Elevate your app's visual appeal with the elegance of CrimsonUI.</Fluent.TextBlock>
        </h2>
        <h3>
          <Fluent.Button variant="hyperlink" onclick="window.location.href='https://ivirius.vercel.app/crimsonui';">Learn more</Fluent.Button>
        </h3>
</section>

<!--Styles-->
<style>
  /*Import theme*/
	/*@import url("https://unpkg.com/fluent-svelte/theme.css");*/
  

	/* Some base styles to get things looking right. */
	:global(body) 
  {
    /*Background color*/
		background-color: var(--fds-solid-background-base);

    /*Background image*/
    background-image: url("https://github.com/IviriusMain/sveltekit-1/blob/main/src%2Froutes%2Fassets%2FBloomRed.png?raw=true");

	/* Accent Colors */
	/*--fds-accent-light-3: 7, 100%, 71%;
  --fds-accent-light-2: 7, 100%, 67%;
  --fds-accent-light-1: 7, 100%, 63%;
  --fds-accent-base: 7, 100%, 54%;
  --fds-accent-dark-1: 7, 100%, 47%;
  --fds-accent-dark-2: 7, 100%, 35%;
  --fds-accent-dark-3: 7, 100%, 27%;
   */ 
    
    /*Background color*/
		color: var(--fds-text-primary); 
	}
  
  /* Global Variables */
:root {
	/* Accent Colors */
	--fds-accent-light-3: 7, 100%, 71% !important;
  --fds-accent-light-2: 7, 100%, 67% !important;
  --fds-accent-light-1: 7, 100%, 63% !important;
  --fds-accent-base: 7, 100%, 54% !important;
  --fds-accent-dark-1: 7, 100%, 47% !important;
  --fds-accent-dark-2: 7, 100%, 35% !important;
  --fds-accent-dark-3: 7, 100%, 27% !important;
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