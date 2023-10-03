<script>
  export let colour
</script>

<div class="input__container" >
  <input type="text" placeholder="Input colour name..." value={ colour } />

  <button type="button">Flip Colour</button>
</div>

<style>
  .input__container {
    width: min(95%, 500px);
    padding: 5px 10px 10px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 10px;

    box-shadow: var(--shadow);
  }

  input {
    padding: 10px 0;
    border-bottom: 1px solid #000;
    width: 100%;
    font-size: 16px;
  }

  button {
    width: 30%;
    background-color: lavender;
    margin-top: 10px;
    border-radius: 5px;
    padding: 10px 5px;
    font-size: 14px;
    font-weight: 500;
    cursor: pointer;
    transition: all .5s;
  }

  button:hover {
    background-color: lavenderblush;
  }

  button:disabled,
  button:disabled:hover {
    background-color: lightgrey;
    color: #888;
    cursor: not-allowed;
  }
</style>