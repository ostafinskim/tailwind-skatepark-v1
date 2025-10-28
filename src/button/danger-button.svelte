<script>
  const { label = 'Button', ...props } = $props();
</script>

<button
  class="rounded-md outline-red-500 border-red-600
 bg-red-300 p-3 text-red-800 shadow hover:underline transition"
  {...props}>{label}</button
>
