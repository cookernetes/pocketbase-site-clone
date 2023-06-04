<script lang="ts">
    import { cn } from "$lib/utils";

    const demoRoutePath = "/collections/users";

    let routes = demoRoutePath.split("/").filter((item) => item !== "");
    routes[0] = routes[0][0].toUpperCase() + routes[0].slice(1);
</script>

<div class="text-xl">
    {#each routes as route, i}
        <a class={cn(i !== routes.length - 1 ? "text-muted-foreground" : "", (i !== 1 || i !== routes.length -1) ? "pr-2" : "")}>{route}</a>
        {#if i < routes.length - 1}
            <span class={cn(i !== routes.length - 1 ? "text-muted-foreground" : "", (i !== 1 || i !== routes.length -1) ? "pr-2" : "")}> / </span>
        {/if}
    {/each}
</div>