<script>
  const { label = 'A Very Important Checkbox', id = 'checkbox', ...props } = $props();
</script>

<div
  class="rounded border bg-slate-200 p-4 outline-offset-2 outline-sky-400 focus-within:bg-sky-200"
>
  <input class="accent-purple-500" {id} {...props} type="checkbox" />
  <label for={id}>{label}</label>
</div>
