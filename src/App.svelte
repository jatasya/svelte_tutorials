<script>
  import EventDemo from "./EventDemo.svelte";
  import Greeting from "./Greeting.svelte";
  import LoginButton from "./LoginButton.svelte";
  import FrameWorksList from "./FrameWorksList.svelte";
  export let name;
</script>

<style>
  main {
    text-align: center;
    padding: 1em;
    max-width: 240px;
    margin: 0 auto;
  }

  h1 {
    color: #ff3e00;
    text-transform: uppercase;
    font-size: 4em;
    font-weight: 100;
  }

  @media (min-width: 640px) {
    main {
      max-width: none;
    }
  }
</style>

<main>
  <LoginButton />
  <h1>Hello {name}!</h1>
  <Greeting first_name="Ashwini" last_name="Vikas" />
  <p>
    Visit the
    <a href="https://svelte.dev/tutorial">Svelte tutorial</a>
    to learn how to build Svelte apps.
  </p>
  <FrameWorksList />
  <EventDemo />
</main>
