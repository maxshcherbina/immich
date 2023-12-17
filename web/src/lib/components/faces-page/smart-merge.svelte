<script lang="ts">
  import Slider from '../elements/slider.svelte';
  import { smartMergeEnabled } from '$lib/stores/preferences.store';
</script>

<div
  title="When enabled, the merged person's name and date of birth are kept if the primary person does not have this information."
  class="flex px-4 gap-2 text-sm"
>
  <p>Smart merge</p>
  <Slider bind:checked={$smartMergeEnabled} />
</div>
