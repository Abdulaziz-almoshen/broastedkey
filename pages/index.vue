<template>
  <!-- component -->
  <div>
    <!--
  This example requires some changes to your config:
  
  ```
  // tailwind.config.js
  module.exports = {
    // ...
    plugins: [
      // ...
      require('@tailwindcss/forms'),
      require('@tailwindcss/aspect-ratio'),
    ],
  }
  ```
-->
    <div class="bg-white">
      <!--
    Mobile menu

    Off-canvas menu for mobile, show/hide based on off-canvas menu state.
  -->
      <div class="relative z-40 lg:hidden" role="dialog" aria-modal="false">
        <!--
      Off-canvas menu backdrop, show/hide based on off-canvas menu state.

      Entering: "transition-opacity ease-linear duration-300"
        From: "opacity-0"
        To: "opacity-100"
      Leaving: "transition-opacity ease-linear duration-300"
        From: "opacity-100"
        To: "opacity-0"
    -->
        <div class="fixed inset-0 bg-black bg-opacity-25"></div>

        <div class="fixed inset-0 z-40 flex">
          <!--
        Off-canvas menu, show/hide based on off-canvas menu state.

        Entering: "transition ease-in-out duration-300 transform"
          From: "-translate-x-full"
          To: "translate-x-0"
        Leaving: "transition ease-in-out duration-300 transform"
          From: "translate-x-0"
          To: "-translate-x-full"
      -->
        </div>
      </div>

      <header class="relative z-10">
        <nav aria-label="Top">
          <!-- Top navigation -->
          <div class="bg-gray-900">
            <div
              class="mx-auto flex h-10 max-w-7xl items-center justify-between px-4 sm:px-6 lg:px-8"
            >
              <!-- Currency selector -->
              <form class="hidden lg:block lg:flex-1">
                <div class="flex">
                  <label for="desktop-currency" class="sr-only">Currency</label>
                  <div
                    class="group relative -ml-2 rounded-md border-transparent bg-gray-900 focus-within:ring-2 focus-within:ring-white"
                  >
                    <select
                      id="desktop-currency"
                      name="currency"
                      class="flex items-center rounded-md border-transparent bg-gray-900 bg-none py-0.5 pl-2 pr-5 text-sm font-medium text-white focus:border-transparent focus:outline-none focus:ring-0 group-hover:text-gray-100"
                    >
                      <option>CAD</option>

                      <option>USD</option>

                      <option>AUD</option>

                      <option>EUR</option>

                      <option>GBP</option>
                    </select>
                    <div
                      class="pointer-events-none absolute inset-y-0 right-0 flex items-center"
                    >
                      <!-- Heroicon name: mini/chevron-down -->
                      <svg
                        class="h-5 w-5 text-gray-300"
                        xmlns="http://www.w3.org/2000/svg"
                        viewBox="0 0 20 20"
                        fill="currentColor"
                        aria-hidden="true"
                      >
                        <path
                          fill-rule="evenodd"
                          d="M5.23 7.21a.75.75 0 011.06.02L10 11.168l3.71-3.938a.75.75 0 111.08 1.04l-4.25 4.5a.75.75 0 01-1.08 0l-4.25-4.5a.75.75 0 01.02-1.06z"
                          clip-rule="evenodd"
                        />
                      </svg>
                    </div>
                  </div>
                </div>
              </form>

              <p
                class="flex-1 text-center text-sm font-medium text-white lg:flex-none"
              >
                Get free delivery on orders over $100
              </p>

              <div
                class="hidden lg:flex lg:flex-1 lg:items-center lg:justify-end lg:space-x-6"
              >
                <a
                  href="#"
                  class="text-sm font-medium text-white hover:text-gray-100"
                  >Create an account</a
                >
                <span class="h-6 w-px bg-gray-600" aria-hidden="true"></span>
                <a
                  href="#"
                  class="text-sm font-medium text-white hover:text-gray-100"
                  >Sign in</a
                >
              </div>
            </div>
          </div>

          <!-- Secondary navigation -->
          <div class="bg-white">
            <div class="border-b border-gray-200">
              <div class="mx-auto max-w-7xl px-4 sm:px-6 lg:px-8">
                <div class="flex h-16 items-center justify-between">
                  <!-- Logo (lg+) -->
                  <div class="hidden lg:flex lg:items-center">
                    <a href="#">
                      <span class="sr-only">Your Company</span>
                      <img
                        class="h-8 w-auto"
                        src="https://scontent.fruh4-6.fna.fbcdn.net/v/t39.30808-6/243547962_1063021347901551_6553224124569965068_n.jpg?_nc_cat=111&ccb=1-7&_nc_sid=09cbfe&_nc_ohc=TREgUPftLoIAX-_hQ5x&_nc_ht=scontent.fruh4-6.fna&oh=00_AfCzNvdtlqvQAXqyQz8kmTexs9zi312js1_zK3MN3oM7ow&oe=63C091C2"
                        alt=""
                      />
                    </a>
                  </div>

                  <div class="hidden h-full lg:flex">
                    <!-- Mega menus -->
                    <div class="ml-8">
                      <div class="flex h-full justify-center space-x-8">
                        <div class="flex">
                          <div class="relative flex">
                            <!-- Item active: "border-indigo-600 text-indigo-600", Item inactive: "border-transparent text-gray-700 hover:text-gray-800" -->
                            <button
                              type="button"
                              class="border-transparent text-gray-700 hover:text-gray-800 relative z-10 -mb-px flex items-center border-b-2 pt-px text-sm font-medium transition-colors duration-200 ease-out"
                              aria-expanded="false"
                            >
                              Women
                            </button>
                          </div>

                          <!--
                        'Women' mega menu, show/hide based on flyout menu state.

                        Entering: "transition ease-out duration-200"
                          From: "opacity-0"
                          To: "opacity-100"
                        Leaving: "transition ease-in duration-150"
                          From: "opacity-100"
                          To: "opacity-0"
                      -->
                          
                        </div>

                        <div class="flex">
                          <div class="relative flex">
                            <!-- Item active: "border-indigo-600 text-indigo-600", Item inactive: "border-transparent text-gray-700 hover:text-gray-800" -->
                            <button
                              type="button"
                              class="border-transparent text-gray-700 hover:text-gray-800 relative z-10 -mb-px flex items-center border-b-2 pt-px text-sm font-medium transition-colors duration-200 ease-out"
                              aria-expanded="false"
                            >
                              Men
                            </button>
                          </div>

                          <!--
                        'Men' mega menu, show/hide based on flyout menu state.

                        Entering: "transition ease-out duration-200"
                          From: "opacity-0"
                          To: "opacity-100"
                        Leaving: "transition ease-in duration-150"
                          From: "opacity-100"
                          To: "opacity-0"
                      -->
                          <div
                            class="absolute inset-x-0 top-full text-gray-500 sm:text-sm"
                          >
                            <!-- Presentational element used to render the bottom shadow, if we put the shadow on the actual panel it pokes out the top, so we use this shorter element to hide the top of the shadow -->
                            <div
                              class="absolute inset-0 top-1/2 bg-white shadow"
                              aria-hidden="true"
                            ></div>

                            
                          </div>
                        </div>

                        <a
                          href="#"
                          class="flex items-center text-sm font-medium text-gray-700 hover:text-gray-800"
                          >Company</a
                        >

                        <a
                          href="#"
                          class="flex items-center text-sm font-medium text-gray-700 hover:text-gray-800"
                          >Stores</a
                        >
                      </div>
                    </div>
                  </div>

                  <!-- Mobile menu and search (lg-) -->
                  <div class="flex flex-1 items-center lg:hidden">
                    <!-- Mobile menu toggle, controls the 'mobileMenuOpen' state. -->
                    <button
                      type="button"
                      class="-ml-2 rounded-md bg-white p-2 text-gray-400"
                    >
                      <span class="sr-only">Open menu</span>
                      <!-- Heroicon name: outline/bars-3 -->
                      <svg
                        class="h-6 w-6"
                        xmlns="http://www.w3.org/2000/svg"
                        fill="none"
                        viewBox="0 0 24 24"
                        stroke-width="1.5"
                        stroke="currentColor"
                        aria-hidden="true"
                      >
                        <path
                          stroke-linecap="round"
                          stroke-linejoin="round"
                          d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5"
                        />
                      </svg>
                    </button>

                    <!-- Search -->
                    <a
                      href="#"
                      class="ml-2 p-2 text-gray-400 hover:text-gray-500"
                    >
                      <span class="sr-only">Search</span>
                      <!-- Heroicon name: outline/magnifying-glass -->
                      <svg
                        class="h-6 w-6"
                        xmlns="http://www.w3.org/2000/svg"
                        fill="none"
                        viewBox="0 0 24 24"
                        stroke-width="1.5"
                        stroke="currentColor"
                        aria-hidden="true"
                      >
                        <path
                          stroke-linecap="round"
                          stroke-linejoin="round"
                          d="M21 21l-5.197-5.197m0 0A7.5 7.5 0 105.196 5.196a7.5 7.5 0 0010.607 10.607z"
                        />
                      </svg>
                    </a>
                  </div>

                  <!-- Logo (lg-) -->
                  <a href="#" class="lg:hidden">
                    <span class="sr-only">Your Company</span>
                    <img
                      src="https://scontent.fruh4-6.fna.fbcdn.net/v/t39.30808-6/243547962_1063021347901551_6553224124569965068_n.jpg?_nc_cat=111&ccb=1-7&_nc_sid=09cbfe&_nc_ohc=TREgUPftLoIAX-_hQ5x&_nc_ht=scontent.fruh4-6.fna&oh=00_AfCzNvdtlqvQAXqyQz8kmTexs9zi312js1_zK3MN3oM7ow&oe=63C091C2"
                      alt="https://scontent.fruh4-6.fna.fbcdn.net/v/t39.30808-6/243547962_1063021347901551_6553224124569965068_n.jpg?_nc_cat=111&ccb=1-7&_nc_sid=09cbfe&_nc_ohc=TREgUPftLoIAX-_hQ5x&_nc_ht=scontent.fruh4-6.fna&oh=00_AfCzNvdtlqvQAXqyQz8kmTexs9zi312js1_zK3MN3oM7ow&oe=63C091C2"
                      class="h-8 w-auto"
                    />
                  </a>

                  <div class="flex flex-1 items-center justify-end">
                    <div class="flex items-center lg:ml-8">
                      <div class="flex space-x-8">
                        <div class="hidden lg:flex">
                          <a
                            href="#"
                            class="-m-2 p-2 text-gray-400 hover:text-gray-500"
                          >
                            <span class="sr-only">Search</span>
                            <!-- Heroicon name: outline/magnifying-glass -->
                            <svg
                              class="h-6 w-6"
                              xmlns="http://www.w3.org/2000/svg"
                              fill="none"
                              viewBox="0 0 24 24"
                              stroke-width="1.5"
                              stroke="currentColor"
                              aria-hidden="true"
                            >
                              <path
                                stroke-linecap="round"
                                stroke-linejoin="round"
                                d="M21 21l-5.197-5.197m0 0A7.5 7.5 0 105.196 5.196a7.5 7.5 0 0010.607 10.607z"
                              />
                            </svg>
                          </a>
                        </div>

                        <div class="flex">
                          <a
                            href="#"
                            class="-m-2 p-2 text-gray-400 hover:text-gray-500"
                          >
                            <span class="sr-only">Account</span>
                            <!-- Heroicon name: outline/user -->
                            <svg
                              class="h-6 w-6"
                              xmlns="http://www.w3.org/2000/svg"
                              fill="none"
                              viewBox="0 0 24 24"
                              stroke-width="1.5"
                              stroke="currentColor"
                              aria-hidden="true"
                            >
                              <path
                                stroke-linecap="round"
                                stroke-linejoin="round"
                                d="M15.75 6a3.75 3.75 0 11-7.5 0 3.75 3.75 0 017.5 0zM4.501 20.118a7.5 7.5 0 0114.998 0A17.933 17.933 0 0112 21.75c-2.676 0-5.216-.584-7.499-1.632z"
                              />
                            </svg>
                          </a>
                        </div>
                      </div>

                      <span
                        class="mx-4 h-6 w-px bg-gray-200 lg:mx-6"
                        aria-hidden="true"
                      ></span>

                      <div class="flow-root">
                        <a href="#" class="group -m-2 flex items-center p-2">
                          <!-- Heroicon name: outline/shopping-cart -->
                          <svg
                            class="h-6 w-6 flex-shrink-0 text-gray-400 group-hover:text-gray-500"
                            xmlns="http://www.w3.org/2000/svg"
                            fill="none"
                            viewBox="0 0 24 24"
                            stroke-width="1.5"
                            stroke="currentColor"
                            aria-hidden="true"
                          >
                            <path
                              stroke-linecap="round"
                              stroke-linejoin="round"
                              d="M2.25 3h1.386c.51 0 .955.343 1.087.835l.383 1.437M7.5 14.25a3 3 0 00-3 3h15.75m-12.75-3h11.218c1.121-2.3 2.1-4.684 2.924-7.138a60.114 60.114 0 00-16.536-1.84M7.5 14.25L5.106 5.272M6 20.25a.75.75 0 11-1.5 0 .75.75 0 011.5 0zm12.75 0a.75.75 0 11-1.5 0 .75.75 0 011.5 0z"
                            />
                          </svg>
                          <span
                            class="ml-2 text-sm font-medium text-gray-700 group-hover:text-gray-800"
                            >0</span
                          >
                          <span class="sr-only">items in cart, view bag</span>
                        </a>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </nav>
      </header>

      <main>
        <!-- Hero -->
        <div class="flex flex-col border-b border-gray-200 lg:border-0">
          <nav aria-label="Offers" class="order-last lg:order-first">
            <div class="mx-auto max-w-7xl lg:px-8">
              <ul
                role="list"
                class="grid grid-cols-1 divide-y divide-gray-200 lg:grid-cols-3 lg:divide-y-0 lg:divide-x"
              >
                <li class="flex flex-col">
                  <a
                    href="#"
                    class="relative flex flex-1 flex-col justify-center bg-white py-6 px-4 text-center focus:z-10"
                  >
                    <p class="text-sm text-gray-500">Download the app</p>
                    <p class="font-semibold text-gray-900">
                      Get an exclusive $5 off code
                    </p>
                  </a>
                </li>

                <li class="flex flex-col">
                  <a
                    href="#"
                    class="relative flex flex-1 flex-col justify-center bg-white py-6 px-4 text-center focus:z-10"
                  >
                    <p class="text-sm text-gray-500">
                      Return when you&#039;re ready
                    </p>
                    <p class="font-semibold text-gray-900">
                      60 days of free returns
                    </p>
                  </a>
                </li>

                <li class="flex flex-col">
                  <a
                    href="#"
                    class="relative flex flex-1 flex-col justify-center bg-white py-6 px-4 text-center focus:z-10"
                  >
                    <p class="text-sm text-gray-500">
                      Sign up for our newsletter
                    </p>
                    <p class="font-semibold text-gray-900">
                      15% off your first order
                    </p>
                  </a>
                </li>
              </ul>
            </div>
          </nav>

          <div class="relative">
            <div
              aria-hidden="true"
              class="absolute hidden h-full w-1/2 bg-gray-100 lg:block"
            ></div>
            <div class="relative bg-gray-100 lg:bg-transparent">
              <div
                class="mx-auto max-w-7xl px-4 sm:px-6 lg:grid lg:grid-cols-2 lg:px-8"
              >
                <div class="mx-auto max-w-2xl py-24 lg:max-w-none lg:py-64">
                  <div class="lg:pr-16">
                    <h1
                      class="text-4xl font-bold tracking-tight text-gray-900 sm:text-5xl xl:text-6xl"
                    >
                      Focus on what matters
                    </h1>
                    <p class="mt-4 text-xl text-gray-600">
                      All the charts, datepickers, and notifications in the
                      world can't beat checking off some items on a paper card.
                    </p>
                    <div class="mt-6">
                      <a
                        href="#"
                        class="inline-block rounded-md border border-transparent bg-indigo-600 py-3 px-8 font-medium text-white hover:bg-indigo-700"
                        >Shop Productivity</a
                      >
                    </div>
                  </div>
                </div>
              </div>
            </div>
            <div
              class="h-48 w-full sm:h-64 lg:absolute lg:top-0 lg:right-0 lg:h-full lg:w-1/2"
            >
              <img
                src="https://scontent.fruh4-6.fna.fbcdn.net/v/t39.30808-6/243547962_1063021347901551_6553224124569965068_n.jpg?_nc_cat=111&ccb=1-7&_nc_sid=09cbfe&_nc_ohc=TREgUPftLoIAX-_hQ5x&_nc_ht=scontent.fruh4-6.fna&oh=00_AfCzNvdtlqvQAXqyQz8kmTexs9zi312js1_zK3MN3oM7ow&oe=63C091C2"
                alt=""
                class="h-full w-full object-cover object-center"
              />
            </div>
          </div>
        </div>

        <!-- Trending products -->
        <section aria-labelledby="trending-heading" class="bg-white">
          <div class="py-16 sm:py-24 lg:mx-auto lg:max-w-7xl lg:py-32 lg:px-8">
            <div class="flex items-center justify-between px-4 sm:px-6 lg:px-0">
              <h2
                id="trending-heading"
                class="text-2xl font-bold tracking-tight text-gray-900"
              >
                Trending products
              </h2>
              <a
                href="#"
                class="hidden text-sm font-semibold text-indigo-600 hover:text-indigo-500 sm:block"
              >
                See everything
                <span aria-hidden="true"> &rarr;</span>
              </a>
            </div>

            <div class="relative mt-8">
              <div class="relative w-full overflow-x-auto">
                <ul
                  role="list"
                  class="mx-4 inline-flex space-x-8 sm:mx-6 lg:mx-0 lg:grid lg:grid-cols-4 lg:gap-x-8 lg:space-x-0"
                >
                  <li class="inline-flex w-64 flex-col text-center lg:w-auto">
                    <div class="group relative">
                      <div
                        class="aspect-w-1 aspect-h-1 w-full overflow-hidden rounded-md bg-gray-200"
                      >
                        <img
                          src="https://scontent.fruh4-5.fna.fbcdn.net/v/t39.30808-6/304763907_496849515782841_1261232390846616750_n.jpg?_nc_cat=110&ccb=1-7&_nc_sid=e3f864&_nc_ohc=lhY5_fmj1sUAX_FBiWb&tn=z5OvhjPnHHWt1509&_nc_ht=scontent.fruh4-5.fna&oh=00_AfC2lM-Zobj2KfbDcjxtXyHF8PbuI9wluefACG89EWuTvA&oe=63C082EE"
                          alt="Black machined steel pen with hexagonal grip and small white logo at top."
                          class="h-full w-full object-cover object-center group-hover:opacity-75"
                        />
                      </div>
                      <div class="mt-6">
                        <p class="text-sm text-gray-500">Spicy</p>
                        <h3 class="mt-1 font-semibold text-gray-900">
                          <a href="#">
                            <span class="absolute inset-0"></span>
                            Spicy Chicken
                          </a>
                        </h3>
                        <p class="mt-1 text-gray-900">$35</p>
                      </div>
                    </div>

                    
                  </li>

                  <!-- More products... -->
                </ul>
              </div>
            </div>

            <div class="mt-12 px-4 sm:hidden">
              <a
                href="#"
                class="text-sm font-semibold text-indigo-600 hover:text-indigo-500"
              >
                See everything
                <span aria-hidden="true"> &rarr;</span>
              </a>
            </div>
          </div>
        </section>

        <!-- Collections -->
        <section aria-labelledby="collections-heading" class="bg-gray-100">
          <div class="mx-auto max-w-7xl px-4 sm:px-6 lg:px-8">
            <div
              class="mx-auto max-w-2xl py-16 sm:py-24 lg:max-w-none lg:py-32"
            >
              <h2
                id="collections-heading"
                class="text-2xl font-bold text-gray-900"
              >
                Collections
              </h2>

              <div
                class="mt-6 space-y-12 lg:grid lg:grid-cols-3 lg:gap-x-6 lg:space-y-0"
              >
                <div class="group relative">
                  <div
                    class="relative h-80 w-full overflow-hidden rounded-lg bg-white group-hover:opacity-75 sm:aspect-w-2 sm:aspect-h-1 sm:h-64 lg:aspect-w-1 lg:aspect-h-1"
                  >
                    <img
                      src="https://scontent.fruh4-6.fna.fbcdn.net/v/t39.30808-6/324231316_5432435623528792_5791606561915341281_n.jpg?_nc_cat=111&ccb=1-7&_nc_sid=8bfeb9&_nc_ohc=uf6yroLmr6EAX9roF1T&tn=z5OvhjPnHHWt1509&_nc_ht=scontent.fruh4-6.fna&oh=00_AfAH20vhq_q0W3q7PDm0ZHQnx1gaQeDHxWeLQ4aiHKi1gA&oe=63C0FBE0"
                      alt="Desk with leather desk pad, walnut desk organizer, wireless keyboard and mouse, and porcelain mug."
                      class="h-full w-full object-cover object-center"
                    />
                  </div>
                  <h3 class="mt-6 text-sm text-gray-500">
                    <a href="#">
                      <span class="absolute inset-0"></span>
                      Black Burger
                    </a>
                  </h3>
                  <p class="text-base font-semibold text-gray-900">
                    Burger
                  </p>
                </div>

                <div class="group relative">
                  <div
                    class="relative h-80 w-full overflow-hidden rounded-lg bg-white group-hover:opacity-75 sm:aspect-w-2 sm:aspect-h-1 sm:h-64 lg:aspect-w-1 lg:aspect-h-1"
                  >
                    <img
                      src="https://scontent.fruh4-5.fna.fbcdn.net/v/t39.30808-6/321610012_902422401138763_7309190368792402520_n.jpg?_nc_cat=110&ccb=1-7&_nc_sid=8bfeb9&_nc_ohc=4h-A4LAmHKwAX9IeCdC&_nc_ht=scontent.fruh4-5.fna&oh=00_AfAP-VW3Dj2M4ypWODMextd-P1TAkz9DYwNI92kLuXnHww&oe=63C1DC83"
                      alt="Wood table with porcelain mug, leather journal, brass pen, leather key ring, and a houseplant."
                      class="h-full w-full object-cover object-center"
                    />
                  </div>
                  <h3 class="mt-6 text-sm text-gray-500">
                    <a href="#">
                      <span class="absolute inset-0"></span>
                      Orange Burger
                    </a>
                  </h3>
                  <p class="text-base font-semibold text-gray-900">
                    Burger
                  </p>
                </div>

                <div class="group relative">
                  <div
                    class="relative h-80 w-full overflow-hidden rounded-lg bg-white group-hover:opacity-75 sm:aspect-w-2 sm:aspect-h-1 sm:h-64 lg:aspect-w-1 lg:aspect-h-1"
                  >
                    <img
                      src="https://scontent.fruh4-4.fna.fbcdn.net/v/t39.30808-6/319776511_586886813445777_8928201418327120033_n.jpg?_nc_cat=104&ccb=1-7&_nc_sid=8bfeb9&_nc_ohc=UPpt6UgKa6wAX8Qi6hD&_nc_ht=scontent.fruh4-4.fna&oh=00_AfDdQFgZVxPB_q9JQZJOmjMzgIk2R4cLClEr7ki2Oqh5eQ&oe=63C1B925"
                      alt="Collection of four insulated travel bottles on wooden shelf."
                      class="h-full w-full object-cover object-center"
                    />
                  </div>
                  <h3 class="mt-6 text-sm text-gray-500">
                    <a href="#">
                      <span class="absolute inset-0"></span>
                      Wings
                    </a>
                  </h3>
                  <p class="text-base font-semibold text-gray-900">
                    Wings
                  </p>
                </div>
              </div>
            </div>
          </div>
        </section>

        <!-- Sale and testimonials -->
        <div class="relative overflow-hidden">
          <!-- Decorative background image and gradient -->
          <div aria-hidden="true" class="absolute inset-0">
            <div
              class="absolute inset-0 mx-auto max-w-7xl overflow-hidden xl:px-8"
            >
              <img
                src="https://tailwindui.com/img/ecommerce-images/home-page-02-sale-full-width.jpg"
                alt=""
                class="h-full w-full object-cover object-center"
              />
            </div>
            <div class="absolute inset-0 bg-white bg-opacity-75"></div>
            <div
              class="absolute inset-0 bg-gradient-to-t from-white via-white"
            ></div>
          </div>

          <!-- Sale -->
          

          <!-- Testimonials -->
          
        </div>
      </main>

      <footer aria-labelledby="footer-heading" class="bg-white">
        <h2 id="footer-heading" class="sr-only">Footer</h2>
        <div class="mx-auto max-w-7xl px-4 sm:px-6 lg:px-8">
          <div class="border-t border-gray-200">
            <div class="pt-16 pb-20">
              <div class="md:flex md:justify-center">
                <img
                  src="https://scontent.fruh4-6.fna.fbcdn.net/v/t39.30808-6/243547962_1063021347901551_6553224124569965068_n.jpg?_nc_cat=111&ccb=1-7&_nc_sid=09cbfe&_nc_ohc=TREgUPftLoIAX-_hQ5x&_nc_ht=scontent.fruh4-6.fna&oh=00_AfCzNvdtlqvQAXqyQz8kmTexs9zi312js1_zK3MN3oM7ow&oe=63C091C2"
                  alt="https://scontent.fruh4-6.fna.fbcdn.net/v/t39.30808-6/243547962_1063021347901551_6553224124569965068_n.jpg?_nc_cat=111&ccb=1-7&_nc_sid=09cbfe&_nc_ohc=TREgUPftLoIAX-_hQ5x&_nc_ht=scontent.fruh4-6.fna&oh=00_AfCzNvdtlqvQAXqyQz8kmTexs9zi312js1_zK3MN3oM7ow&oe=63C091C2"
                  class="h-8 w-auto"
                />
              </div>
              <div
                class="mx-auto mt-16 max-w-5xl xl:grid xl:grid-cols-2 xl:gap-8"
              >
                <div class="grid grid-cols-2 gap-8 xl:col-span-2">
                  <div
                    class="space-y-12 md:grid md:grid-cols-2 md:gap-8 md:space-y-0"
                  >
                    <div>
                      <h3 class="text-sm font-medium text-gray-900">
                        Products
                      </h3>
                      <ul role="list" class="mt-6 space-y-6">
                        <li class="text-sm">
                          <a href="#" class="text-gray-500 hover:text-gray-600"
                            >Bags</a
                          >
                        </li>

                        <li class="text-sm">
                          <a href="#" class="text-gray-500 hover:text-gray-600"
                            >Tees</a
                          >
                        </li>

                        <li class="text-sm">
                          <a href="#" class="text-gray-500 hover:text-gray-600"
                            >Objects</a
                          >
                        </li>

                        <li class="text-sm">
                          <a href="#" class="text-gray-500 hover:text-gray-600"
                            >Home Goods</a
                          >
                        </li>

                        <li class="text-sm">
                          <a href="#" class="text-gray-500 hover:text-gray-600"
                            >Accessories</a
                          >
                        </li>
                      </ul>
                    </div>
                    <div>
                      <h3 class="text-sm font-medium text-gray-900">
                        Customer Service
                      </h3>
                      <ul role="list" class="mt-6 space-y-6">
                        <li class="text-sm">
                          <a href="#" class="text-gray-500 hover:text-gray-600"
                            >Contact</a
                          >
                        </li>

                        <li class="text-sm">
                          <a href="#" class="text-gray-500 hover:text-gray-600"
                            >Shipping</a
                          >
                        </li>

                        <li class="text-sm">
                          <a href="#" class="text-gray-500 hover:text-gray-600"
                            >Returns</a
                          >
                        </li>

                        <li class="text-sm">
                          <a href="#" class="text-gray-500 hover:text-gray-600"
                            >Warranty</a
                          >
                        </li>

                        <li class="text-sm">
                          <a href="#" class="text-gray-500 hover:text-gray-600"
                            >Secure Payments</a
                          >
                        </li>

                        <li class="text-sm">
                          <a href="#" class="text-gray-500 hover:text-gray-600"
                            >FAQ</a
                          >
                        </li>

                        <li class="text-sm">
                          <a href="#" class="text-gray-500 hover:text-gray-600"
                            >Find a store</a
                          >
                        </li>
                      </ul>
                    </div>
                  </div>
                  <div
                    class="space-y-12 md:grid md:grid-cols-2 md:gap-8 md:space-y-0"
                  >
                    <div>
                      <h3 class="text-sm font-medium text-gray-900">Company</h3>
                      <ul role="list" class="mt-6 space-y-6">
                        <li class="text-sm">
                          <a href="#" class="text-gray-500 hover:text-gray-600"
                            >Who we are</a
                          >
                        </li>

                        <li class="text-sm">
                          <a href="#" class="text-gray-500 hover:text-gray-600"
                            >Sustainability</a
                          >
                        </li>

                        <li class="text-sm">
                          <a href="#" class="text-gray-500 hover:text-gray-600"
                            >Press</a
                          >
                        </li>

                        <li class="text-sm">
                          <a href="#" class="text-gray-500 hover:text-gray-600"
                            >Careers</a
                          >
                        </li>

                        <li class="text-sm">
                          <a href="#" class="text-gray-500 hover:text-gray-600"
                            >Terms &amp; Conditions</a
                          >
                        </li>

                        <li class="text-sm">
                          <a href="#" class="text-gray-500 hover:text-gray-600"
                            >Privacy</a
                          >
                        </li>
                      </ul>
                    </div>
                    <div>
                      <h3 class="text-sm font-medium text-gray-900">Legal</h3>
                      <ul role="list" class="mt-6 space-y-6">
                        <li class="text-sm">
                          <a href="#" class="text-gray-500 hover:text-gray-600"
                            >Terms of Service</a
                          >
                        </li>

                        <li class="text-sm">
                          <a href="#" class="text-gray-500 hover:text-gray-600"
                            >Return Policy</a
                          >
                        </li>

                        <li class="text-sm">
                          <a href="#" class="text-gray-500 hover:text-gray-600"
                            >Privacy Policy</a
                          >
                        </li>

                        <li class="text-sm">
                          <a href="#" class="text-gray-500 hover:text-gray-600"
                            >Shipping Policy</a
                          >
                        </li>
                      </ul>
                    </div>
                  </div>
                </div>
              </div>
            </div>

            <div class="lg:grid lg:grid-cols-2 lg:gap-x-6 xl:gap-x-8">
              <div class="flex items-center rounded-lg bg-gray-100 p-6 sm:p-10">
                <div class="mx-auto max-w-sm">
                  <h3 class="font-semibold text-gray-900">
                    Sign up for our newsletter
                  </h3>
                  <p class="mt-2 text-sm text-gray-500">
                    The latest news, articles, and resources, sent to your inbox
                    weekly.
                  </p>
                  <form class="mt-4 sm:mt-6 sm:flex">
                    <label for="email-address" class="sr-only"
                      >Email address</label
                    >
                    <input
                      id="email-address"
                      type="text"
                      autocomplete="email"
                      required
                      class="w-full min-w-0 appearance-none rounded-md border border-gray-300 bg-white py-2 px-4 text-base text-gray-900 placeholder-gray-500 shadow-sm focus:border-indigo-500 focus:outline-none focus:ring-1 focus:ring-indigo-500"
                    />
                    <div class="mt-3 sm:mt-0 sm:ml-4 sm:flex-shrink-0">
                      <button
                        type="submit"
                        class="flex w-full items-center justify-center rounded-md border border-transparent bg-indigo-600 py-2 px-4 text-base font-medium text-white shadow-sm hover:bg-indigo-700 focus:outline-none focus:ring-2 focus:ring-indigo-500 focus:ring-offset-2 focus:ring-offset-white"
                      >
                        Sign up
                      </button>
                    </div>
                  </form>
                </div>
              </div>

              <div
                class="relative mt-6 flex items-center py-12 px-6 sm:py-16 sm:px-10 lg:mt-0"
              >
                <div class="absolute inset-0 overflow-hidden rounded-lg">
                  <img
                    src="https://tailwindui.com/img/ecommerce-images/footer-02-exclusive-sale.jpg"
                    alt=""
                    class="h-full w-full object-cover object-center saturate-0 filter"
                  />
                  <div
                    class="absolute inset-0 bg-indigo-600 bg-opacity-90"
                  ></div>
                </div>
                <div class="relative mx-auto max-w-sm text-center">
                  <h3 class="text-2xl font-bold tracking-tight text-white">
                    Get early access
                  </h3>
                  <p class="mt-2 text-gray-200">
                    Did you sign up to the newsletter? If so, use the keyword we
                    sent you to get access.
                    <a
                      href="#"
                      class="whitespace-nowrap font-bold text-white hover:text-gray-200"
                      >Go now<span aria-hidden="true"> &rarr;</span></a
                    >
                  </p>
                </div>
              </div>
            </div>
          </div>

          <div class="py-10 md:flex md:items-center md:justify-between">
            <div class="text-center md:text-left">
              <p class="text-sm text-gray-500">
                &copy; 2023 All Rights Reserved Dar Kataket Restaurants Company
                - One Individual Company
              </p>
              <p class="text-sm text-gray-500">Commercial Number: 101074712</p>
              <p class="text-sm text-gray-500">Phone Number: +966540680389</p>
              <p class="text-sm text-gray-500">
                Address: :7936 Haroun Al Rashid Al Jazeerah Dist.3906
              </p>
            </div>

            <div class="mt-4 flex items-center justify-center md:mt-0">
              <div class="flex space-x-8">
                <a href="#" class="text-sm text-gray-500 hover:text-gray-600"
                  >Accessibility</a
                >

                <a href="#" class="text-sm text-gray-500 hover:text-gray-600"
                  >Privacy</a
                >

                <a href="#" class="text-sm text-gray-500 hover:text-gray-600"
                  >Terms</a
                >
              </div>

              <div class="ml-6 border-l border-gray-200 pl-6">
                <a
                  href="#"
                  class="flex items-center text-gray-500 hover:text-gray-600"
                >
                  <img
                    src="https://icons.iconarchive.com/icons/wikipedia/flags/72/SA-Saudi-Arabia-Flag-icon.png"
                    alt=""
                    class="h-auto w-5 flex-shrink-0"
                  />
                  <span class="ml-3 text-sm">Change</span>
                  <span class="sr-only">location and currency</span>
                </a>
              </div>
            </div>
          </div>
        </div>
      </footer>
    </div>
  </div>
</template>

<script>
export default {}
</script>
