<script lang="ts">
  import { ArgumentType } from '../classes/ArgumentType';
  export var type: ArgumentType;
</script>

<div class="mt-4">
  <svg
    xmlns="http://www.w3.org/2000/svg"
    class="h-10 w-10 stroke-current text-green-500 m-auto"
    fill="none"
    viewBox="0 0 24 24"
    stroke="currentColor"
  >
    <path
      stroke-linecap="round"
      stroke-linejoin="round"
      stroke-width="2"
      d="M12 9v3m0 0v3m0-3h3m-3 0H9m12 0a9 9 0 11-18 0 9 9 0 0118 0z"
    />
  </svg>

  <div class="p-4 m-4 border-2 border-green-200 bg-green-100 rounded-lg w-96">
    <details>
      <summary>Nice looking is better!</summary>
      <p>If the dummy looks nice, everything should look nice!</p>
    </details>
  </div>
  <p>{type}</p>
</div>
