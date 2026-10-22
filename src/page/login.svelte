<script>
  import TextField from '../lib/TextField.svelte'
  import SecretField from '../lib/SecretField.svelte'

  let nombre = $state('')
  let clave = $state('')

  function enviar(event) {
    event.preventDefault()
    console.log({ nombre, clave })
  }
</script>

<h1>Login</h1>

<form onsubmit={enviar}>
  <TextField label="Nombre" placeholder="Escribe tu nombre" bind:value={nombre} />
  <SecretField label="Contraseña" placeholder="Escribe tu contraseña" bind:value={clave} />
  <button type="submit">Enviar</button>
</form>
