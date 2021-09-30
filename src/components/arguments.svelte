<script lang="ts">
  import Negative from '$src/svgs/contra.svelte';
  import Positive from '$src/svgs/pro.svelte';
  import { ArgumentType } from '../classes/ArgumentType';

  export var type: ArgumentType;
  var borderColor: string = '';
  var bgColor: string = '';
  if (type == ArgumentType.Pro) {
    borderColor = 'border-green-200';
    bgColor = 'bg-green-100';
  } else {
    borderColor = 'border-red-200';
    bgColor = 'bg-red-100';
  }
</script>

<div class="mt-4">
  {#if type == ArgumentType.Pro}
    <Positive />
  {:else}
    <Negative />
  {/if}

  <div class="p-4 m-4 border-2 rounded-lg w-96 {borderColor} {bgColor}">
    <details>
      <summary class="text-lg">Nice looking is better!</summary>
      <p>If the dummy looks nice, everything should look nice!</p>
    </details>
    <details>
      <summary>Second Argument</summary>
      <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsa quidem aspernatur sit quaerat
        error ea praesentium doloremque similique fugit placeat. Reprehenderit, tempora? Molestiae
        pariatur natus cupiditate nihil facere autem et!
      </p>
    </details>
  </div>
</div>
