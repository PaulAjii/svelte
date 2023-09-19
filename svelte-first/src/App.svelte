<script>
  import Counter from "./lib/Counter.svelte"

  let name = "Svelte Counter"
</script>

<div class="container">
  <h1>{ name }</h1>
  <Counter />
</div>

<style>
  .container h1 {
    text-align: center;
  }
</style>

