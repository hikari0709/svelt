<script>
  import main from './assets/main.png'
  import Section from './lib/Content.svelte'
</script>

<main class="body">
  <img src={main} alt="main visual" />
  <Section />
</main>

<style>
  .body {
    background-color: #f7f3e8;
  }
</style>
