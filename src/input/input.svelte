<script>
  const { id = 'input', label, description, error, ...props } = $props();
  const descriptionId = description ? `${id}-description` : undefined;
  const errorId = error ? `${id}-error` : undefined;
</script>

<div class="space-y-1.5">
  <label class="block font-medium text-slate-700" for={id}>{label}</label>
  <input
    class="block rounded px-2 py-1.5 outline outline-offset-2 outline-slate-600 placeholder:italic user-invalid:outline-red-500 focus:outline-2 focus:outline-blue-500"
    {id}
    aria-describedby={descriptionId}
    aria-invalid={!!error}
    aria-errormessage={errorId}
    {...props}
  />
  {#if description}
    <p id={descriptionId}>{description}</p>
  {/if}
  {#if error}
    <p id={errorId}>{error}</p>
  {/if}
</div>
