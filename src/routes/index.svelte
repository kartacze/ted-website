<script>
  import { fade } from "svelte/transition";
</script>

<style>
  .wrapper {
    height: 100%;
    width: 100%;
  }

  h1,
  h2,
  p {
    text-align: center;
    margin: 0 auto;
  }

  h1 {
    font-size: 2.8em;
    text-transform: uppercase;
    font-weight: 700;
    margin: 0 0 0.5em 0;
  }

  h2 {
    font-size: 1.8em;
    text-transform: uppercase;
    font-weight: 700;
    margin: 0 0 0.5em 0;
  }

  p {
    margin: 1em auto;
  }

  @media (min-width: 480px) {
    h1 {
      font-size: 4em;
    }
  }

  div {
    width: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
    margin: auto;
  }
</style>

<svelte:head>
  <title>Utile - Teodor Pytka</title>
  <meta
    name="description"
    content="Utile - Teodor Pytka - Software developer who is currently building web apps with React / Svelte"
  />
</svelte:head>

<div class="wrapper" transition:fade style="position:absolute">
  <h1>Utile</h1>
  <h2>Teodor Pytka</h2>

  <p>
    Building web apps using React / Svelte.
  </p>
</div>
