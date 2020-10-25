<script>
  import {onMount} from 'svelte';
  import { onDestroy } from 'svelte';

  export let sdk;

  onMount(() => {
    console.log('starting window resizer');
    sdk.window.startAutoResizer();
  });

  onDestroy(() => {
    console.log('stopping window resizer');
    sdk.window.stopAutoResizer();
  });

</script>

<p>This is a sidebar component</p>