<script>
  const { title = 'Card Title', description = '' } = $props();
</script>

<div class="max-w-fit m-auto shadow rounded-lg outline-violet-600 outline border-slate-400 p-8 text-center space-y-5">
  <h2 class="font-black underline underline-offset-7 text-4xl">{title}</h2>
  <p class="text-2xl">{description}</p>
</div>
