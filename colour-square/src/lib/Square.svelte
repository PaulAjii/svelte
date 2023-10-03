<script>
  export let colour
</script>

<div class="square">
  <p class="colour__name">
    { colour }
  </p>
</div>

<style>
  .square {
    width: min(90%, 500px);
    height: 300px;
    border: 2px solid white;
    border-radius: 10px;
    margin-bottom: 1.5rem;

    display: grid;
    place-content: center;

    box-shadow: var(--shadow);
  }

  .colour__name {
    font-size: 20px;
    font-weight: 600;
  }
</style>
