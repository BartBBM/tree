<script>
  import { ArgumentType } from '$src/classes/ArgumentType';

  import Arguments from '$src/components/arguments.svelte';
</script>

<div class="py-12">
  <div class="text-center">
    <h2 class="text-xl text-indigo-600">Dummy</h2>
    <h1 class="text-3xl mt-2 font-semibold">Should the Dummy look nice?</h1>
  </div>

  <div class="flex justify-evenly bg-gray-100 rounded-3xl mt-8">
    <Arguments type={ArgumentType.Pro} />
    <Arguments type={ArgumentType.Contra} />
  </div>
</div>
