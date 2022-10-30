<template>
  <!-- component -->
  <div>
    <div class="relative w-full">
      <nav class="fixed z-10 w-full bg-white md:absolute md:bg-transparent">
        <div class="container m-auto px-2 md:px-12 lg:px-7">
          <div
            class="flex flex-wrap items-center justify-between py-3 gap-6 md:py-4 md:gap-0"
          >
            <div class="w-full px-6 flex justify-between lg:w-max md:px-0">
              <a
                href="https://tailus.io/blocks/hero-section"
                aria-label="logo"
                class="flex space-x-2 items-center"
              >
                <img
                  src="https://tailus.io/sources/blocks/food-delivery/preview/images/icon.png"
                  class="w-12"
                  alt="tailus logo"
                  width="144"
                  height="133"
                />
                <span class="text-2xl font-bold text-yellow-900"
                  >Broasted <span class="text-yellow-700">Key</span></span
                >
              </a>
              <button
                aria-label="humburger"
                id="hamburger"
                class="relative w-10 h-10 -mr-2 lg:hidden"
              >
                <div
                  aria-hidden="true"
                  id="line"
                  class="inset-0 w-6 h-0.5 m-auto rounded bg-yellow-900 transtion duration-300"
                ></div>
                <div
                  aria-hidden="true"
                  id="line2"
                  class="inset-0 w-6 h-0.5 mt-2 m-auto rounded bg-yellow-900 transtion duration-300"
                ></div>
              </button>
            </div>
            <div
              class="hidden w-full lg:flex flex-wrap justify-end items-center space-y-6 p-6 rounded-xl bg-white md:space-y-0 md:p-0 md:flex-nowrap md:bg-transparent lg:w-7/12"
            >
              <div class="text-gray-600 lg:pr-4">
                <ul
                  class="space-y-6 tracking-wide font-medium text-sm md:flex md:space-y-0"
                >
                  <li>
                    <a
                      href="#"
                      class="block md:px-4 transition hover:text-yellow-700"
                    >
                      <span>I've a restaurant</span>
                    </a>
                  </li>
                  <li>
                    <a
                      href="#"
                      class="block md:px-4 transition hover:text-yellow-700"
                    >
                      <span>Wishlist</span>
                    </a>
                  </li>
                  <li>
                    <a
                      href="#"
                      class="block md:px-4 transition hover:text-yellow-700"
                    >
                      <span>Cart</span>
                    </a>
                  </li>
                </ul>
              </div>
              <div
                class="w-full space-y-2 border-yellow-200 lg:space-y-0 md:w-max lg:border-l"
              >
                <button
                  type="button"
                  title="Start buying"
                  class="w-full py-3 px-6 text-center rounded-full transition active:bg-yellow-200 focus:bg-yellow-100 sm:w-max"
                >
                  <span class="block text-yellow-800 font-semibold text-sm">
                    Sign up
                  </span>
                </button>
                <button
                  type="button"
                  title="Start buying"
                  class="w-full py-3 px-6 text-center rounded-full transition bg-yellow-300 hover:bg-yellow-100 active:bg-yellow-400 focus:bg-yellow-300 sm:w-max"
                >
                  <span class="block text-yellow-900 font-semibold text-sm">
                    Login
                  </span>
                </button>
              </div>
            </div>
          </div>
        </div>
      </nav>
      <div class="relative bg-yellow-50">
        <div
          class="container m-auto px-6 pt-32 md:px-12 lg:pt-[4.8rem] lg:px-7"
        >
          <div class="flex items-center flex-wrap px-2 md:px-0">
            <div class="relative lg:w-6/12 lg:py-24 xl:py-32">
              <h1
                class="font-bold text-4xl text-yellow-900 md:text-5xl lg:w-10/12"
              >
                Your favorite dishes, right at your door
              </h1>
              <form action="" class="w-full mt-12">
                <div
                  class="relative flex p-1 rounded-full bg-white border border-yellow-200 shadow-md md:p-2"
                >
                  <select
                    class="hidden p-3 rounded-full bg-transparent md:block md:p-4"
                    name="domain"
                    id="domain"
                  >
                    <option value="design">FastFood</option>
                    <option value="development">Restaurant</option>
                    <option value="marketing">Marketing</option>
                  </select>
                  <input
                    placeholder="Your favorite food"
                    class="w-full p-4 rounded-full"
                    type="text"
                  />
                  <button
                    type="button"
                    title="Start buying"
                    class="ml-auto py-3 px-6 rounded-full text-center transition bg-gradient-to-b from-yellow-200 to-yellow-300 hover:to-red-300 active:from-yellow-400 focus:from-red-400 md:px-12"
                  >
                    <span class="hidden text-yellow-900 font-semibold md:block">
                      Search
                    </span>
                    <svg
                      xmlns="http://www.w3.org/2000/svg"
                      class="w-5 mx-auto text-yellow-900 md:hidden"
                      fill="currentColor"
                      viewBox="0 0 16 16"
                    >
                      <path
                        d="M11.742 10.344a6.5 6.5 0 1 0-1.397 1.398h-.001c.03.04.062.078.098.115l3.85 3.85a1 1 0 0 0 1.415-1.414l-3.85-3.85a1.007 1.007 0 0 0-.115-.1zM12 6.5a5.5 5.5 0 1 1-11 0 5.5 5.5 0 0 1 11 0z"
                      />
                    </svg>
                  </button>
                </div>
              </form>
              <p class="mt-8 text-gray-700 lg:w-10/12">
                Sit amet consectetur adipisicing elit.
                <a href="#" class="text-yellow-700">connection</a> tenetur nihil
                quaerat suscipit, sunt dignissimos.
              </p>
            </div>
            <div class="ml-auto -mb-24 lg:-mb-56 lg:w-6/12">
              <img
                src="https://tailus.io/sources/blocks/food-delivery/preview/images/food.webp"
                class="relative"
                alt="food illustration"
                loading="lazy"
                width="4500"
                height="4500"
              />
            </div>
          </div>
        </div>
      </div>
    </div>

    <footer
      class="px-3 py-8 bg-white dark:bg-gray-800 text-2 text-gray-500 dark:text-gray-200 transition-colors duration-200"
    >
      <div class="flex flex-col">
        <div class="md:hidden mt-7 mx-auto w-11 h-px rounded-full"></div>
        <div class="mt-4 md:mt-0 flex flex-col md:flex-row">
          <nav
            class="flex-1 flex flex-col items-center justify-center md:items-end md:border-r border-gray-100 md:pr-5"
          >
            <a
              aria-current="page"
              href="#"
              class="hover:text-gray-700 dark:hover:text-white"
            >
              مطاعم دار كتاكيت للوجبات السريعة <br>
              ٧٩٣٦،هارون الرشيد. الجزيرة، ٣٩-٦
            </a>
            <a
              aria-current="page"
              href="#"
              class="hover:text-gray-700 dark:hover:text-white"
            >
              Contacts
            </a>
            <a
              aria-current="page"
              href="#"
              class="hover:text-gray-700 dark:hover:text-white"
            >
              Customization
            </a>
          </nav>
          <div class="md:hidden mt-4 mx-auto w-11 h-px rounded-full"></div>
          <div
            class="mt-4 md:mt-0 flex-1 flex items-center justify-center md:border-r border-gray-100"
          >
            <a
              class="hover:text-primary-gray-20"
              href="https://github.com/Charlie85270/tail-kit"
            >
              <span class="sr-only"> View on GitHub </span>
              <svg
                xmlns="http://www.w3.org/2000/svg"
                width="30"
                height="30"
                fill="currentColor"
                class="text-xl hover:text-gray-800 dark:hover:text-white transition-colors duration-200"
                viewBox="0 0 1792 1792"
              >
                <path
                  d="M896 128q209 0 385.5 103t279.5 279.5 103 385.5q0 251-146.5 451.5t-378.5 277.5q-27 5-40-7t-13-30q0-3 .5-76.5t.5-134.5q0-97-52-142 57-6 102.5-18t94-39 81-66.5 53-105 20.5-150.5q0-119-79-206 37-91-8-204-28-9-81 11t-92 44l-38 24q-93-26-192-26t-192 26q-16-11-42.5-27t-83.5-38.5-85-13.5q-45 113-8 204-79 87-79 206 0 85 20.5 150t52.5 105 80.5 67 94 39 102.5 18q-39 36-49 103-21 10-45 15t-57 5-65.5-21.5-55.5-62.5q-19-32-48.5-52t-49.5-24l-20-3q-21 0-29 4.5t-5 11.5 9 14 13 12l7 5q22 10 43.5 38t31.5 51l10 23q13 38 44 61.5t67 30 69.5 7 55.5-3.5l23-4q0 38 .5 88.5t.5 54.5q0 18-13 30t-40 7q-232-77-378.5-277.5t-146.5-451.5q0-209 103-385.5t279.5-279.5 385.5-103zm-477 1103q3-7-7-12-10-3-13 2-3 7 7 12 9 6 13-2zm31 34q7-5-2-16-10-9-16-3-7 5 2 16 10 10 16 3zm30 45q9-7 0-19-8-13-17-6-9 5 0 18t17 7zm42 42q8-8-4-19-12-12-20-3-9 8 4 19 12 12 20 3zm57 25q3-11-13-16-15-4-19 7t13 15q15 6 19-6zm63 5q0-13-17-11-16 0-16 11 0 13 17 11 16 0 16-11zm58-10q-2-11-18-9-16 3-14 15t18 8 14-14z"
                ></path>
              </svg>
            </a>
            <a class="ml-4 hover:text-primary-gray-20" href="#">
              <span class="sr-only"> Settings </span>
              <svg
                width="30"
                height="30"
                fill="currentColor"
                class="text-xl hover:text-gray-800 dark:hover:text-white transition-colors duration-200"
                viewBox="0 0 2048 1792"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M960 896q0-106-75-181t-181-75-181 75-75 181 75 181 181 75 181-75 75-181zm768 512q0-52-38-90t-90-38-90 38-38 90q0 53 37.5 90.5t90.5 37.5 90.5-37.5 37.5-90.5zm0-1024q0-52-38-90t-90-38-90 38-38 90q0 53 37.5 90.5t90.5 37.5 90.5-37.5 37.5-90.5zm-384 421v185q0 10-7 19.5t-16 10.5l-155 24q-11 35-32 76 34 48 90 115 7 11 7 20 0 12-7 19-23 30-82.5 89.5t-78.5 59.5q-11 0-21-7l-115-90q-37 19-77 31-11 108-23 155-7 24-30 24h-186q-11 0-20-7.5t-10-17.5l-23-153q-34-10-75-31l-118 89q-7 7-20 7-11 0-21-8-144-133-144-160 0-9 7-19 10-14 41-53t47-61q-23-44-35-82l-152-24q-10-1-17-9.5t-7-19.5v-185q0-10 7-19.5t16-10.5l155-24q11-35 32-76-34-48-90-115-7-11-7-20 0-12 7-20 22-30 82-89t79-59q11 0 21 7l115 90q34-18 77-32 11-108 23-154 7-24 30-24h186q11 0 20 7.5t10 17.5l23 153q34 10 75 31l118-89q8-7 20-7 11 0 21 8 144 133 144 160 0 8-7 19-12 16-42 54t-45 60q23 48 34 82l152 23q10 2 17 10.5t7 19.5zm640 533v140q0 16-149 31-12 27-30 52 51 113 51 138 0 4-4 7-122 71-124 71-8 0-46-47t-52-68q-20 2-30 2t-30-2q-14 21-52 68t-46 47q-2 0-124-71-4-3-4-7 0-25 51-138-18-25-30-52-149-15-149-31v-140q0-16 149-31 13-29 30-52-51-113-51-138 0-4 4-7 4-2 35-20t59-34 30-16q8 0 46 46.5t52 67.5q20-2 30-2t30 2q51-71 92-112l6-2q4 0 124 70 4 3 4 7 0 25-51 138 17 23 30 52 149 15 149 31zm0-1024v140q0 16-149 31-12 27-30 52 51 113 51 138 0 4-4 7-122 71-124 71-8 0-46-47t-52-68q-20 2-30 2t-30-2q-14 21-52 68t-46 47q-2 0-124-71-4-3-4-7 0-25 51-138-18-25-30-52-149-15-149-31v-140q0-16 149-31 13-29 30-52-51-113-51-138 0-4 4-7 4-2 35-20t59-34 30-16q8 0 46 46.5t52 67.5q20-2 30-2t30 2q51-71 92-112l6-2q4 0 124 70 4 3 4 7 0 25-51 138 17 23 30 52 149 15 149 31z"
                ></path>
              </svg>
            </a>
          </div>
          <div class="md:hidden mt-4 mx-auto w-11 h-px rounded-full"></div>
          <div
            class="mt-8 md:mt-0 flex-1 flex flex-col items-center justify-center md:items-start md:pl-5"
          >
            
          </div>
        </div>
      </div>
    </footer>
  </div>
</template>

<script>
export default {}
</script>
