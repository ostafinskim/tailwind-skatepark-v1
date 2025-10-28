<script>
  const { label = 'Button', ...props } = $props();
</script>

<button
  class="rounded-md bg-purple-600 px-4 py-2 font-black text-white shadow hover:bg-white hover:text-purple-600"
  {...props}>{label}</button
>
