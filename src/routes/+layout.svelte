<script lang="ts">
      import "../app.scss";
      import Navbar from '../components/Navbar.svelte';
</script>

<div>
    <Navbar />
</div>
<div>
    <h1 class="text-3xl font-bold underline text-red-400">
        Hello world!
      </h1>
    <slot />
</div>