

  <script>
    let showMenu = false;
  
    function toggleNavbar() {
      showMenu = !showMenu;
    }
  
    function closeNavbar() {
      showMenu = false;
    }

  </script>
  
  <div class="bg-gray-900">
   <div>
      <nav
        class="p-4 px-6 mx-auto shadow-lg md:flex md:justify-between md:items-center"
      >
        <div class="flex items-center justify-between">
          <a href="/" class="flex items-center">
            <img src="/showerpowerbrand.webp" class="h-14 w-14 hover:scale-105 duration-500" alt="iDrew Logo" />
          </a>
  
          <!-- Mobile menu button -->
          <div class="flex md:hidden">
            <button
              type="button"
              class="text-white hover:text-gray focus:outline-none focus:text-gray-400"
              aria-label="Toggle Navigation"
              on:click={toggleNavbar}
            >
              <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="white" class="w-6 h-6">
                <path stroke-linecap="round" stroke-linejoin="round" d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5" />
              </svg>
            </button>
          </div>
        </div>
  
        <!-- Mobile Menu open: "block", Menu closed: "hidden" -->
        <div
          class="flex-col mt-8 space-y-4 md:flex md:space-y-0 md:flex-row md:items-center md:justify-center md:space-x-6 lg:space-x-12 md:mt-0 {showMenu ? 'flex' : 'hidden'}"
        >
          <a class="text-gray-500 duration-500 hover:text-opacity-70  hover:underline ease-in-out" href="/volunteer" on:click={closeNavbar}>Volunteer</a>
          <a class="text-gray-500 duration-500 hover:text-opacity-70  hover:underline ease-in-out" href="/aboutus" on:click={closeNavbar}>About Us</a>
          <a class="text-gray-500 duration-500 hover:text-opacity-70  hover:underline ease-in-out" href="/sponsors" on:click={closeNavbar}>Sponsors</a>
          <a class="text-gray-500 duration-500 hover:text-opacity-70  hover:underline ease-in-out" href="https://www.bonfire.com/store/gobelove-swag/" on:click={closeNavbar}>#GOBELOVE</a>
          <a class="text-gray-500 duration-500 hover:text-opacity-70  hover:underline ease-in-out" href="/contactus" on:click={closeNavbar}>Contact</a>
          <a href="https://showerpower.kindful.com/" class="text-gray-500 duration-500 hover:text-opacity-70  hover:underline ease-in-out md:bg-red-500 md:px-4 md:py-2 rounded-md md:text-white block md:hidden">Donate</a>


        
        </div>
        <a href="https://showerpower.kindful.com/" class="bg-red-500 px-4 py-2 rounded-md text-white hidden md:block hover:opacity-80 ease-out duration-300">Donate</a>
        
      </nav>
    </div>
  </div>