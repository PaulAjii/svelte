<script>
  import Square from './lib/Square.svelte'
  import Input from './lib/Input.svelte'

  let colourName = ""
</script>

<h1>Colour Square</h1>
<p>{colourName}</p>
  <Square colour={ colourName } />
  <Input colour={colourName} />