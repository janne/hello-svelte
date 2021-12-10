<script lang="ts">
  export let value: number = 0;
  export let step: number = 1;
</script>

<div>
  <slot>Default Counter</slot>
  <div>
    <button on:click={() => (value -= step)}>-</button>
    {value}
    <button on:click={() => (value += step)}>+</button>
  </div>
</div>
