<script lang="ts">
    const message = `Contact Page`;
    let reactive = 0;
    let userName = '';
    const updateState = (event: PointerEvent) => {
        reactive ++;
        console.log(userName);
    }
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
