<script>
  let { label = '', value = $bindable(''), placeholder = '', type = 'text' } = $props()
</script>

<label>
  {label}
  <input {type} {placeholder} bind:value />
</label>
