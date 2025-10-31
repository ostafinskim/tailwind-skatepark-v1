<script module>
  import { defineMeta } from '@storybook/addon-svelte-csf';
  import FileTree from './file-tree.svelte';

  const { Story } = defineMeta({
    title: 'FileTree',
    component: FileTree,
  });
</script>

<Story name="Default" />
