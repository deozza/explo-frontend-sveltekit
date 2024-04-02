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
