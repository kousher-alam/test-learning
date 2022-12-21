<script lang="ts">
      import "../app.scss";
</script>
<div>
    <nav>
        <ul>
            <li><a href="/">Home</a></li>
            <li><a href="/about">About</a></li>
            <li><a href="/contact">Contact</a></li>
        </ul>
    </nav>
</div>

<div>
    <h1 class="text-3xl font-bold underline text-red-400">
        Hello world!
      </h1>
    <slot />
</div>