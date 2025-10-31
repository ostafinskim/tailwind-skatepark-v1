<script>
  const { label = 'A Very Important Checkbox', id = 'checkbox', ...props } = $props();
</script>

<div class="group border bg-slate-200 p-4 has-checked:bg-green-300">
  <input class="accent-purple-500" {id} {...props} type="checkbox" />
  <label class="group-has-checked:line-through" for={id}>{label}</label>
  <div class="hidden gap-2 group-has-checked:flex">
    <label>What is your reason</label>
    <input
      required
      class="mt-4 block w-full rounded bg-white px-2 py-1 placeholder-slate-500 outline outline-slate-600 placeholder:font-light user-invalid:outline-red-600 focus:outline-2 focus:outline-blue-600"
      type="text"
    />
    <button class="group-has-[input:invalid]:hidden">Submit</button>
  </div>
</div>
