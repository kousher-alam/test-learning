<script lang="ts">
    const message = `Contact Page`;
    let reactive = 0;
    let userName = '';
    const updateState = (event: PointerEvent) => {
        reactive ++;
        console.log(userName);
    }
    const lines = [
        "line 1",
        "line 1",
        "line 1",
        "line 1",
        "line 1",
        "line 1",
        "line 1",
        "line 1",
    ]
</script>

<style lang="scss">
    h1 {
        color: red;
    }
</style>

<h1>{message}</h1>
<input type="text" bind:value={userName}/>
<p>{userName}</p>
<button on:click={updateState}>{reactive}</button>
<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>
<div>
    {#each lines as line}
        <h2 class=" text-5xl capitalize">{line}</h2>
    {/each}
</div>
