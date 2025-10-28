<script>
  const { label = 'Button', ...props } = $props();
</script>

<button
  class="rounded-md bg-purple-300 px-4 py-2 font-black shadow text-shadow-black hover:bg-black hover:text-purple-100"
  {...props}>{label}</button
>
