<script>
  export let title
  export let bg_color
</script>

<button style="background-color: {bg_color}" type="button" on:click>
  { title }
</button>

<style>
  button {
    color: white;
    padding: 8px 15px;
    border-radius: 5px;
    font-weight: 700;
    cursor: pointer;
    transition: 0.5s;
  }

  button:hover {
    scale: 1.02;
  }
</style>