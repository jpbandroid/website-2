<script lang="ts">
	//Imports
	import * as Fluent from 'fluent-svelte';
	import 'fluent-svelte/theme.css';

	//Variables
	let openTooShortMsg = false;
  let openTooShortSub = false;

	let email = '';
	let subject = '';
	let message = '';

  function validateEmail(email) {
    const re = /\S+@\S+\.\S+/;
    return re.test(email);
  }

	async function sendToDiscord() {

    if (!validateEmail(email)) {
      // add the code to show the email is not valid message
      console.error('Email is not valid!');
      return;
    }

		if (subject.length < 5) {
      // add the code to show the subject is not valid message
			console.error('Subject must be alteast 5 characters long!');
			return;
		}

    if (message.length < 25) {
      // add the code to show the message is not valid message
      console.error('Message must be alteast 25 characters long!');
      openTooShortMsg = true;
      return;
    }

		const webhookUrl = '';
		const payload = new FormData();
    payload.append('email', email);
    payload.append('subject', subject);
    payload.append('message', message);

		try {
      const response = await fetch(webhookUrl, {
        method: 'POST',
        body: payload
      });

      if (!response.ok) {
        if (response.status === 429) {
          // add the code to show the rate limited message
          console.error('Rate limited!');
          return;
        }
        else {
          // add the code to show the failed to send message
          console.error('Failed to send message!');
          return;
        }
      }

      const data = await response.json();
      console.log(data);
    } catch (error) {
      // add the code to show the error message
      console.error('Error:', error);
    }

    // clear the form
    email = '';
    subject = '';
    message = '';
	}
</script>

<!--Head-->
<svelte:head>
	<title>ErrorTek's Website</title>
	<meta name="description" content="My official website"/>
</svelte:head>

<!--Navbar-->
<section style="display: flex; flex-wrap: wrap; align-items: center; justify-content: flex-start; padding: 10px; background: rgba(25, 25, 25, 0.15); border-bottom: 1px solid rgba(205, 205, 205, 0.25);">
	<Fluent.PersonPicture src="https://yt3.googleusercontent.com/82KcuEjHraSZUui5_XY4uQj0uUgtcFr1G2DKlpGXyPIlJqd8uAunQqM5mG95sXdTbfqSqL1Npw=s176-c-k-c0x00ffffff-no-rj" style="width: 35px; height: 35px; margin-right: 15px; margin-left: 15px; margin-top: 18px; align-items: center;"/>

	<Fluent.Button style="height: 32px; margin-right: 15px; align-items: center;" variant="hyperlink" onclick="window.location.href='https://errortek.vercel.app';">Home</Fluent.Button>
	<Fluent.Button style="height: 32px; margin-right: 15px; align-items: center;" variant="hyperlink" onclick="window.location.href='https://errortek.vercel.app/crimsonui';">CrimsonUI</Fluent.Button>
	<Fluent.Button style="height: 32px; margin-right: 15px; align-items: center;" variant="hyperlink" onclick="window.location.href='https://errortek.vercel.app/documentations';">Documentations</Fluent.Button>
	<Fluent.Button style="height: 32px; margin-right: 15px; align-items: center;" variant="hyperlink" onclick="window.location.href='https://errortek-news.vercel.app';">News/Blog</Fluent.Button>
	<Fluent.Button style="height: 32px; margin-right: 15px; align-items: center;">Contact</Fluent.Button>
	<Fluent.Button style="height: 32px; margin-right: 15px; align-items: center;" variant="hyperlink" onclick="window.location.href='https://errortek.vercel.app/about';">About</Fluent.Button>
</section>

<!--Title-->
<section class="centered-section">
	<h1>
		<Fluent.TextBlock variant="titleLarge">Contact</Fluent.TextBlock>
	</h1>
</section>

<!--Ivirius Text Editor Plus-->
<section class="margin-section">
  <h1>
<Fluent.InfoBar title="Error!" severity="critical" message="Message is too short." bind:openTooShortMsg />
	  <Fluent.InfoBar title="Error!" severity="caution" message="This area of the site is not finished yet." />

  </h1>
	<h1>
		<Fluent.TextBox
			placeholder="Email"
			type="email"
			style="width: 100%; box-sizing: border-box;"
			bind:value={email}
		/>
	</h1>
	<h2>
		<Fluent.TextBox
			placeholder="Subject"
			style="width: 100%; box-sizing: border-box;"
			bind:value={subject}
		/>
	</h2>
	<h3>
		<Fluent.TextBox
			placeholder="Message"
			style="min-height: 150px; width: 100%; box-sizing: border-box;"
			bind:value={message}
		/>
	</h3>
</section>

<section class="right-section">
	<Fluent.Button style="width: 60px; float: right;" variant="accent" on:click={sendToDiscord}>
		Send
	</Fluent.Button>
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
	@import url('https://unpkg.com/fluent-svelte/theme.css');

	/* Some base styles to get things looking right. */
	:global(body) {
		/*Background color*/
		background-color: var(--fds-solid-background-base);

		/*Background image*/
		background-image: url('https://i.spoo.me/825520');

		/*Background color*/
		color: var(--fds-text-primary);
	}

	/*Centered section*/
	.centered-section {
		text-align: center;
		margin: 0 auto;
		padding: 25px;
		max-width: 1250px;
	}

	/*Right aligned section*/
	.right-section {
		text-align: right;
		margin: auto;
		padding: 25px;
		max-width: 1250px;
		display: flex;
		justify-content: flex-end;
		justify-items: flex-end;
	}

	/*Left aligned centered section*/
	.margin-section {
		margin: 0 auto;
		padding: 25px;
		max-width: 1250px;
	}
</style>
