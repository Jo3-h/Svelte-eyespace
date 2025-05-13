<!-- src/lib/components/Navbar.svelte -->

<script>
    import NavLink from '$lib/components/NavLink.svelte';
</script>

<div class="flex w-full h-20 bg-objects text-white font-bold items-center justify-between">
    <div class="flex w-1/3 h-full"></div>
    <a href='/' class="flex w-1/3 h-full items-center justify-center text-3xl italic">Custom Svelte Web App</a>
    <div class="flex w-1/3 h-full items-center justify-end gap-x-5 px-4">
        <NavLink href="/" text="Home" />
        <NavLink href="/about" text="About" />
        <NavLink href="/contact" text="Contact" />
        <NavLink href="/login" text="Login" />
        
    </div>
    
</div>

