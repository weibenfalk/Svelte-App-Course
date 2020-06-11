<script>
  import { createEventDispatcher } from 'svelte';
  const dispatch = createEventDispatcher();
</script>

<button on:click={() => dispatch('loadMore')}>
  <slot />
</button>

<style>
  button {
    background: #000;
    width: 25%;
    min-width: 200px;
    height: 70px;
    color: #fff;
    cursor: pointer;
    transition: all 0.3s;
    border-radius: 40px;
    font-size: 28px;
    max-width: 1280px;
    display: block;
    margin: 20px auto;
    padding: 0 20px;
    outline: none;
  }

  button:hover {
    opacity: 0.8;
  }
</style>
