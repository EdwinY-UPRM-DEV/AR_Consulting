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

<div class="absolute flex-col top-10 bg-white rounded-2xl shadow-xl max-w-120 max-h-30 p-5 space-y-4 justify-center items-center">      
      <div class='flex space-x-60'>
      <h2 class="text-s font-bold">Card Title</h2>
      <svg xmlns="http://www.w3.org/2000/svg" class="w-5 h-5" fill="none" viewBox="0 0 24 24" stroke="currentColor">
        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7" />
      </svg>
      </div>
      <div class=" flex text-gray-600">This card has an image, title, text, and a button.</div>

