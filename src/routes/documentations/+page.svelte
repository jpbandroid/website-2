<script>
  //Imports
  import * as Fluent from "fluent-svelte";
  import "fluent-svelte/theme.css";
</script>

<!--Head-->
<svelte:head>
        <title>ErrorTek's Website</title>
        <meta name="description" content="ET's documentation" />
</svelte:head>

<section style="display: flex; flex-wrap: wrap; align-items: center; justify-content: flex-start; padding: 10px; background: rgba(25, 25, 25, 0.15); border-bottom: 1px solid rgba(205, 205, 205, 0.25);">
  <Fluent.PersonPicture src="https://yt3.googleusercontent.com/82KcuEjHraSZUui5_XY4uQj0uUgtcFr1G2DKlpGXyPIlJqd8uAunQqM5mG95sXdTbfqSqL1Npw=s176-c-k-c0x00ffffff-no-rj" style="width: 35px; height: 35px; margin-right: 15px; margin-left: 15px; margin-top: 18px; align-items: center;"/>

  <Fluent.Button style="height: 32px; margin-right: 15px; align-items: center;" variant="hyperlink" onclick="window.location.href='https://errortek.vercel.app';">Home</Fluent.Button>
  <Fluent.Button style="height: 32px; margin-right: 15px; align-items: center;" variant="hyperlink" onclick="window.location.href='https://errortek.vercel.app/crimsonui';">CrimsonUI</Fluent.Button>
  <Fluent.Button style="height: 32px; margin-right: 15px; align-items: center;">Documentations</Fluent.Button>
	<Fluent.Button style="height: 32px; margin-right: 15px; align-items: center;" variant="hyperlink" onclick="window.location.href='https://errortek-news.vercel.app';">News/Blog</Fluent.Button>
  <Fluent.Button style="height: 32px; margin-right: 15px; align-items: center;" variant="hyperlink" onclick="window.location.href='https://errortek.vercel.app/contact';">Contact us</Fluent.Button>
  <Fluent.Button style="height: 32px; margin-right: 15px; align-items: center;" variant="hyperlink" onclick="window.location.href='https://errortek.vercel.app/about';">About</Fluent.Button>
</section>

<!--Title-->
<section class="centered-section">
  <h1>
    <Fluent.TextBlock variant="titleLarge">Documentations</Fluent.TextBlock>
  </h1>
 <h2>
                <Fluent.TextBlock variant="body" align="center">
					Find documentations for various tools developed by me or where I am a contributor (for example CrimsonUI)
				</Fluent.TextBlock>
 </h2>
</section>

<section class="margin-section">
        <h2>
  <Fluent.ListItem onclick="window.location.href='https://errortek.vercel.app/crimsonui';">CrimsonUI</Fluent.ListItem>
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
    background-image: url("https://i.spoo.me/825520");

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