<script>
  let { label = '', value = $bindable(''), placeholder = '' } = $props()
</script>

<label>
  {label}
  <input type="password" {placeholder} bind:value />
</label>
