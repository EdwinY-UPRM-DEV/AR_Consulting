<script lang="ts">
  import menuBar from '/burger.svg'
  import companyLogo from '/A_R.png'


  let isOpen = false;
  let isHovered = false;

  function toggleMenu() {
    isOpen = !isOpen;
  }

  const handleEnter = () => isHovered = true;
  const handleLeave = () => isHovered = false;

</script>

<main class='min-h-screen bg-secondary overflow-hidden'>
  <nav id='topNav'class='relative bg-primary h-25 w-screen flex items-center justify-between px-7 shadow-xl text-xl font-bold z-3 '>
    <div>
    <button
      type="button"
      on:click={toggleMenu}
      class='flex items-center justify-center text-white text-center outline-secondary_accent hover:outline-2 bg-gray-650 bg-clip-border outline-offset-4 rounded focus:bg-gray-600 focus:outline-2' >
      <img class='invert w-6 h-6 mr-2' src={menuBar}>
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
  

  <nav id='fullMenu' class='relative h-60 w-2/3 mx-auto bottom-50 flex justify-center items-start bg-primary_accent rounded-b-3xl shadow-xl/20 z-2 transition delay-150 ease-in-out duration-300 {isHovered ? 'translate-y-50' : 'translate-y-0'}'>

    
    <div 
    id="hoverZone" 
    role="button"
    aria-label="Open Nav"
    tabindex="0"
    on:mouseenter={handleEnter}
    on:mouseleave={handleLeave}
    class="absolute top-0 left-1/100 h-60 w-[15%] z-30 {isHovered ? 'w-full h-70' : 'w-[15%] h-60'}">
  </div>  



  
  <div id='menuCards' class='flex absolute min-w-full min-h-full'>
    <div class='flex justify-center space-x-20 min-w-full min-h-full'>

    <div class="flex relative flex-col top-10 bg-white rounded-2xl shadow-xl max-w-120 max-h-30 p-5 space-y-4 justify-center items-center">      
      <div class='flex space-x-60'>
      <h2 class="text-s font-bold">Card Title</h2>
      <svg xmlns="http://www.w3.org/2000/svg" class="w-5 h-5" fill="none" viewBox="0 0 24 24" stroke="currentColor">
        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7" />
      </svg>
      </div>
      <div class=" flex text-aa">This card has an image, title, text, and a button.</div>
    </div>
    
    <div class="flex relative flex-col top-10 bg-white rounded-2xl shadow-xl max-w-120 max-h-30 p-5 space-y-4 justify-center items-center">      
      <div class='flex space-x-60'>
        <h2 class="text-s font-bold">Card Title 2</h2>
        <svg xmlns="http://www.w3.org/2000/svg" class="w-5 h-5" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7" />
        </svg>
      </div>
      <div class="flex text-gray-600">This card has an image, title, text, and a button.
      </div>
    </div>
  </div>
  
</div>

  <div id='menuSelection'>
      <ul class='relative flex text-s text-white space-x-5 sm:space-x-10 md:space-x-20 lg:space-x-35 {isHovered ? 'mt-48 transition-discrete ease-in-out delay-200' : 'mt-52 transition-discrete ease-in-out delay-200'}' >
      <li><a href="#" class=" hover:text-blue-600">Home</a></li>
      <li><a href="#" class=" hover:text-blue-600">About</a></li>
      <li><a href="#" class=" hover:text-blue-600">Services</a></li>
      <li><a href="#" class=" hover:text-blue-600">Overview</a></li>
    </ul>
    </div>
  </nav>



</main>
