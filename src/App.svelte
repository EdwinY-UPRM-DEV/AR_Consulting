<script lang="ts">
  import svelteLogo from './assets/svelte.svg'
  import viteLogo from '/vite.svg'
  import Counter from './lib/Counter.svelte'

  let isOpen = false;

  function toggleMenu() {
    isOpen = !isOpen;
  }
</script>

<main class='min-h-screen bg-blue-500'>
  <nav class='bg-amber-950 flex justify-center items-center '>
    <button
      type="button"
      on:click={toggleMenu}
      class='text-white'>
        <span>Explore</span>
        <svg></svg>
    </button>
    


    <div>
    <img src='#' alt='logo'>
    </div>

    <div> 
      <button
      type='button'
      on:click={toggleMenu}
      class='text-white '>
        <span>Schedule</span>
        <svg></svg>
        </button>
    </div>

  </nav>
</main>