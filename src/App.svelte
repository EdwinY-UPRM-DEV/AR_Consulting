<script lang="ts">
  import menuBar from '/burger.svg'
  import companyLogo from '/A_R.png'
  import hero_img from '/better_hero.png'


  let isOpen = false;
  let isHovered = false;

  function toggleMenu() {
    isOpen = !isOpen;
  }

  const handleEnter = () => isHovered = true;
  const handleLeave = () => isHovered = false;

</script>

<main>
<section style={`background-image: url(${hero_img})`} class='no-scrollbars flex flex-col min-h-[90vh] bg-black/90 bg-cover bg-no-repeat bg-blend-overlay bg-fixed'> 
<!---Nav Bar Container--->
<div class='flex relative h-28 bg-white'>
  <!--Nav Bar Items-->
  <div class='flex justify-start items-center'>
    <img src={companyLogo} class='w-24 h-24 ml-12' alt='A&R Consulting'>
  </div>
  <div class='absolute flex left-1/2 -translate-x-1/2 items-center top-12 gap-8 text-md'>
    <a href='#'>Home</a>
    <a href='#'>Services</a>
    <a href='#'>About Us</a>
    <a href='#'>FAQ</a>
  </div>
</div>
<!--Hero Section Container-->
<div class='flex flex-1 items-start mt-42'>
  <div class=' text-white mx-54 text-start'>
    <h1 class='text-7xl font-bold '>From <span class=' text-blue-400 font-extrabold'>Vision </span> to <span class=' text-red-400 font-extrabold'>Execution.</span></h1>
    <h1 class='text-7xl font-bold'> We  <span class='bg-gradient-to-r from-blue-400 via-indigo-400 to-red-400 bg-clip-text text-transparent font-extrabold'>Bridge </span> the gap.</h1>
    <p class='text-2xl font-light mt-5'>Welcome to A&R Consulting Group,<br> your global partner in executive coaching and consulting. </p>
    <button href='#' class='mt-8 text-lg px-4 py-3 border-inherit rounded-sm bg-blue-400 '> Get Started </button>
  </div>
</div>

</section>
<section class='min-h-screen'>
  
</section>


</main>
