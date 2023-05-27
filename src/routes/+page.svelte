<script lang="ts">
  import type { PageData } from "./$types";
  export let data: PageData;
</script>

<svelte:head>
  <title>林ベーカリー</title>
  <meta name="description" content="Svelte demo app" />
</svelte:head>

<section>
  <h1>ブログ2</h1>
  <ul>
    {#each data.contents as content}
      <li><a href="{content.id}">{content.title}</a></li>
    {/each}
  </ul>
</section>

<style>
  section {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
</style>
  



<!-- <h1>Welcome to SvelteKit</h1>
<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p> -->
