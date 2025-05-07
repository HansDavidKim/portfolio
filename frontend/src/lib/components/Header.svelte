<header class="bg-black">
    <!-- bg-black: Sets the background color of the header to black -->
    <nav 
      class="mx-auto flex max-w-7xl items-center justify-between p-6 lg:px-8" 
      aria-label="Global">
      <!-- 
        mx-auto: Centers the navigation container horizontally
        flex: Enables Flexbox layout for child elements
        max-w-7xl: Sets the maximum width of the navigation to 1280px (7xl)
        items-center: Vertically aligns items to the center
        justify-between: Distributes items with space between (left & right)
        p-6: Applies padding of 1.5rem (24px) on all sides
        lg:px-8: Increases horizontal padding to 2rem (32px) on large screens
      -->
  
      <div class="flex lg:flex-1">
        <!-- 
          flex: Applies Flexbox layout to align items in a row
          lg:flex-1: On large screens, allows the flex item to grow and take full width
        -->
        <a href="/" class="-m-1.5 p-1.5">
          <!-- 
            -m-1.5: Applies negative margin of -0.375rem (-6px)
            p-1.5: Adds padding of 0.375rem (6px)
          -->
          <span class="sr-only">Your Company</span>
          <img 
            class="h-8 w-auto" 
            src="https://tailwindcss.com/plus-assets/img/logos/mark.svg?color=indigo&shade=600" 
            alt="Company Logo">
          <!-- 
            h-8: Sets height to 2rem (32px)
            w-auto: Width is auto-scaled to maintain aspect ratio
          -->
        </a>
      </div>
  
      <!-- Mobile Menu Button (Visible only on small screens) -->
      <div class="flex lg:hidden">
        <!-- 
          flex: Flexbox layout for the button
          lg:hidden: Hides this element on large screens (≥1024px)
        -->
        <button 
          type="button" 
          class="-m-2.5 inline-flex items-center justify-center rounded-md p-2.5 text-white">
          <!-- 
            -m-2.5: Negative margin of -0.625rem (-10px)
            inline-flex: Makes the button an inline flex container
            items-center: Vertically centers the icon in the button
            justify-center: Horizontally centers the icon
            rounded-md: Medium rounded corners (0.375rem)
            p-2.5: Padding of 0.625rem (10px) on all sides
            text-gray-700: Sets text color to medium gray
          -->
          <span class="sr-only">Open main menu</span>
          <svg class="size-6" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" aria-hidden="true">
            <path stroke-linecap="round" stroke-linejoin="round" d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5" />
            <!-- 
              size-6: Sets width and height of SVG to 1.5rem (24px)
              fill="none": No background fill
              stroke-width="1.5": Line thickness of 1.5px
              stroke="currentColor": Follows the text color of the parent (text-gray-700)
            -->
          </svg>
        </button>
      </div>
  
      <!-- Desktop Navigation Menu (Visible on large screens) -->
      <div class="hidden lg:flex lg:gap-x-12">
        <!-- 
          hidden: Hides the menu on small screens
          lg:flex: Shows the menu as a flex container on large screens
          lg:gap-x-12: Horizontal gap of 3rem (48px) between items
        -->
        <a href="/about" class="text-sm/6 font-semibold text-white">About Me</a>
        <!-- 
          text-sm/6: Sets font size to 0.875rem (14px) with line-height 1.5rem (24px)
          font-semibold: Applies medium font weight (600)
          text-gray-900: Text color is dark gray
        -->
        <a href="#" class="text-sm/6 font-semibold text-white">Posts</a>
        <a href="#" class="text-sm/6 font-semibold text-white">Career</a>
      </div>
  
      <!-- Right Section: Log in Button -->
      <div class="hidden lg:flex lg:flex-1 lg:justify-end">
        <!-- 
          hidden: Hides this section on small screens
          lg:flex: Shows this section on large screens as a flex container
          lg:flex-1: Takes the remaining available space
          lg:justify-end: Aligns the content to the right
        -->
        <a href="#" class="text-sm/6 font-semibold text-white">
          GitHub<!--<span aria-hidden="true">&rarr;</span>-->
        </a>
      </div>
    </nav>
  
    <!-- Mobile Menu Panel (Visible only on small screens) -->
    <div class="lg:hidden" role="dialog" aria-modal="true">
      <!-- 
        lg:hidden: Hides the mobile menu on large screens
      -->
      <div class="fixed inset-0 z-10"></div>
      <!-- 
        fixed: Positions the backdrop at a fixed position (does not scroll with page)
        inset-0: Positions it to cover the entire viewport
        z-10: Sets a high stacking order to ensure it appears above other content
      -->
  
      <div class="fixed inset-y-0 right-0 z-10 w-full overflow-y-auto bg-white px-6 py-6 sm:max-w-sm sm:ring-1 sm:ring-gray-900/10">
        <!-- 
          fixed: Positions the menu panel at a fixed position
          inset-y-0: Takes full vertical height
          right-0: Aligns it to the right edge
          w-full: Takes full width (on small screens)
          overflow-y-auto: Allows vertical scrolling if content overflows
          bg-white: Background color is white
          px-6 py-6: Padding of 1.5rem (24px) on all sides
          sm:max-w-sm: Maximum width of 24rem (384px) on small screens
          sm:ring-1 sm:ring-gray-900/10: Applies a subtle shadow around the menu
        -->
      </div>
    </div>
  </header>
  