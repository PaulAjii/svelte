<script>
  import ActionBtn from "./ActionBtn.svelte";

  let count = 0
  $: doubledValue = count * 2
  const  properties = [
  {
    title: "Increment",
    color: "green",
    action() {
      count = count += 1
    }
  },

  {
    title: "Reset",
    color: "blue",
    action() {
      count = count = 0
    }
  },

  {
    title: "Decrement",
    color: "red",
    action() {
      count = count -= 1
    }
  },
]

</script>

<h1>{ count }</h1>
<p>Count doubled is: { doubledValue }</p>

<div class="btn__container">
  {#each properties as btn}
    <ActionBtn
      title={ btn.title }
      bg_color={ btn.color }
      on:click={() => btn.action()}
    />
  {/each}
</div>

<style>
    h1 {
    text-align: center;
    font-size: 8rem;
    font-weight: 900;
  }

  p {
    text-align: center;
    font-weight: 600;
    margin-bottom: 10px;
  }

  .btn__container {
    display: flex;
    gap: 10px;
  }
</style>