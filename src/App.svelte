<script lang="ts">
  import svelteLogo from './assets/svelte.svg'
  import viteLogo from '/vite.svg'
  import plusIcon from '/plus.svg'
  import menuBar from '/burger.svg'
  import companyLogo from '/A_R.png'
  import Counter from './lib/Counter.svelte'

  let isOpen = false;

  function toggleMenu() {
    isOpen = !isOpen;
  }
</script>

<main class='min-h-screen bg-gray-900'>
  <nav class='relative bg-gradient-to-b from-blue-900 to-neutral-600 h-25 w-screen flex items-center justify-between px-7 border-blue-950 border-1 text-xl font-bold z-3 '>

    <div>
    <button
      type="button"
      on:click={toggleMenu}
      class='flex items-center justify-center text-white text-center outline-gray-600 hover:outline-2 bg-gray-650 bg-clip-border outline-offset-4 rounded focus:bg-gray-600 focus:outline-2' >
      <img class=' invert w-6 h-6 mr-2' src={menuBar}>
      <span>Explore</span>
    </button>
    </div>
    


    <div class='absolute left-1/2 transform -translate-x-1/2 flex justify-center items-center'>
    <img class='w-16 h-16' src={companyLogo} alt='logo'>
    </div>

    <div> 
      <button
      type='button'
      on:click={toggleMenu}
      class='text-white flex items-center justify-center text-center gap-0 underline'>
        <span>Schedule Now</span>
        </button>
    </div>

  </nav>
  <nav class='relative h-10 w-2/3 mx-auto bottom-3 flex justify-center items-center bg-slate-700 rounded-b-3xl shadow-xl/20 z-2 hover:bottom-0 hover:h-30'>
    <div>
    </div>
    <div>
      </div>

  </nav>
</main>