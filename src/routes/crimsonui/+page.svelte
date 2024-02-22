<script>
        import * as Fluent from "fluent-svelte";
        import "fluent-svelte/theme.css";
</script>

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

<section class="centered-section">
        <h1>
                <Fluent.TextBlock variant="titleLarge">CrimsonUI</Fluent.TextBlock>
        </h1>
 <h2>
                <Fluent.TextBlock variant="body" align="center">A beautiful and modern UI library the seamlessly combines elements of Fluent design and Aero, as well as taking inspiration from GlowUI.</Fluent.TextBlock>
 </h2>
</section>

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

<style>
    @import url("https://unpkg.com/fluent-svelte/theme.css");

    /* Some base styles to get things looking right. */
    :global(body) {
        background-color: var(--fds-solid-background-base);
        color: var(--fds-text-primary);
    }

    :root {
        --fds-accent-light-3: hsl(7, 100%, 71%);
        --fds-accent-light-2: hsl(7, 100%, 67%);
        --fds-accent-light-1: hsl(7, 100%, 63%);
        --fds-accent-base: hsl(7, 100%, 54%);
        --fds-accent-dark-1: hsl(7, 100%, 41%);
        --fds-accent-dark-2: hsl(7, 100%, 35%);
        --fds-accent-dark-3: hsl(7, 100%, 27%);
    }

    .centered-section {
        text-align: center;
        margin: 25px;
    }

    .margin-section {
        margin: 25px;
    }
</style>
