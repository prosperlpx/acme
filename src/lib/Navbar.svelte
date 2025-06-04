<script>
  import {Link} from 'svelte-routing';
  let isMenuCLose = false;

  function toggleMenu(){
    isMenuCLose = !isMenuCLose
  }
</script>


<header class="sticky top-0 z-10 bg-teal-700 text-white">

  <section class="mx-auto flex max-w-4xl items-center justify-between p-4">
    <h1 class="text-3xl font-medium">
      <a href="#heros">🚀 Acme Rockets</a>
    </h1>

    {#if !isMenuCLose}
      <button class="text-4xl font-bold outline-none md:hidden cursor-pointer"
      on:click={toggleMenu}
      >
          &#9776;
      </button>
    {:else}
        <button class="text-4xl cursor-pointer font-medium md:hidden" on:click={toggleMenu}>
        &times;
        </button> 
    {/if} 

    <nav class="hidden md:inline space-x-8 text-xl font-medium">
          <a href="#rockets" class="hover:opacity-90 active:opacity-80">Our Rockets</a>
          <a href="#socials" class="hover:opacity-90 active:opacity-80">Socials</a>
          <a href="#contact" class="hover:opacity-90 active:opacity-80">Contact Us</a>
    </nav>
  </section>

  {#if isMenuCLose}
    <section class = "justify-center absolute md:hidden w-full flex-col bg-black text-5xl font-medium">
      <nav class="flex min-h-screen flex-col items-center py-8">
        <a href="#heros" class="w-full py-6 text-center hover:opacity-90">Home</a>
        <a href="#rockets" class="w-full py-6 text-center hover:opacity-90">Our Rockets</a>
        <a href="#socials" class="w-full py-6 text-center hover:opacity-90">Socials</a>
        <a href="#contact" class="w-full py-6 text-center hover:opacity-90">Contact Us</a>
      </nav>
    </section>
  {/if}
      

</header>
