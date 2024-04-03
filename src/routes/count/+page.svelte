<script lang="ts">
    let count: number = 0;

    function increment() {
        count += 1;
    }

    function decrement() {
        count -= 1;
    }

</script>

<h1>Count</h1>

<button on:click={decrement}>-</button>
<p>Count: {count}</p>
<button on:click={increment}>+</button>

{#if count % 2 === 0}
    <p>Count is even</p>
{:else}
    <p>Count is odd</p>
{/if}