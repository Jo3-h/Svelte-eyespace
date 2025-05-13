<!-- src/lib/components/NavLink.svelte -->

<script lang="ts">
    export let href: string;
    export let text: string;
</script>


<a href={href} class="px-2 h-2/3 w-15 text flex items-center justify-center
hover:font-extrabold hover:cursor-pointer
">{text}</a>