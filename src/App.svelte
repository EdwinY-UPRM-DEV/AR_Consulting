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

<main class='flex-row relative h-screen w-screen'>
  <nav class='flex bg-amber-300 justify-start items-center min-h-30'>
    <div class='mx-5'>logo </div>
  </nav>

  <div class='relative flex min-h-90 bg-blue-400 '> 
    <div class='absolute flex bg-green-400 justify-center items-center inset-x-30 top-10 bottom-45 outline-3 '> </div>

  </div>
  <div class='absolute flex inset-x-50 bottom-120 top-90 items-center justify-center bg-amber-600 outline-2'>computer</div>




</main>
