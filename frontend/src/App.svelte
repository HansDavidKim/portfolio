<script>
    let name = 'World';
    $: fullName = 'John ' + name;
    import {count} from './store.js';
    let testArray = [1, 2, 3];
</script>
<main>
    <h1>Hello, {name}!</h1>
    <button on:click={() => 
    {
        if (name === 'World') {
            name = 'Svelte';
        } else {
            name = 'World';
        }
    }
    }>Change Name</button>
    <h2>Full Name: {fullName}</h2>
    {#each testArray as item}
        <p>{item}</p>
    {/each}
    <h2>Count: {$count}</h2>
    <button on:click={() => count.update(n => n + 1)}>Increment</button>
    <button on:click={() => count.update(n => n - 1)}>Decrement</button>
</main>