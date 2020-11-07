<script>
  import Tailwindcss from "./Tailwindcss.svelte";
  export let name;
  export let mynum = "42";
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

  .myclassy {
    @apply text-red-700 text-5xl;
  }

  @media (min-width: 640px) {
    main {
      max-width: none;
    }
  }
</style>

<Tailwindcss />

<main>
  <h1>Hello {name}!</h1>
  <p>The meaning of life is <span class="myclassy">{mynum}</span></p>
</main>
