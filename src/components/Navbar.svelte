<script>
    function onBodyClick() {
        console.log('clicked');
    }
</script>
<style lang="scss">
    :global(body) {
        @apply bg-slate-100 w-full min-h-screen;
    }
</style>

<svelte:body on:click={onBodyClick}/>

<div class="p-3 bg-blue-600 text-white fixed w-full top-0 left-0">
    <nav class="">
        <ul class=" flex content-center align-middle shadow-lg">
            <li><a href="/">Home</a></li>
            <li><a href="/about">About</a></li>
            <li><a href="/contact">Contact</a></li>
        </ul>
    </nav>
</div>