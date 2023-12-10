<template>
  <div class="h-screen " :style="getBackgroundStyle()">
    <div class="lg:text-lg lg:flex justify-center text-center space-x-24 pt-16 text-white ">
      <div class="lg:mb-0 ">
        <nuxt-link to="/">
          <img class="w-[120px] h-[120px]" src="~/assets/FlyAir.png" alt="FlyAir Travel Agency">
        </nuxt-link>
      </div>
      <div class="lg:mb-0 mb-4">
        <!-- Dropdown menu -->
        <div class="relative group">
          <span class="cursor-pointer">OUR SERVICES<i class="fa fa-angle-down"></i></span>
          <ul class="hidden absolute top-full left-0 bg-white border border-gray-300 p-4 group-hover:block">
            <li>
              <nuxt-link class="block w-[230px] py-1 text-blue-500 hover:bg-gray-200" to="/air-travel-ticket">Air Tickets</nuxt-link>
            </li>
            <li>
              <nuxt-link class="block w-[230px] py-1 text-blue-500 hover:bg-gray-200" to="/car-hire-airport-transfers">Car Hire & Airport Transfers</nuxt-link>
            </li>
            <li>
              <nuxt-link class="block w-[230px] py-1 text-blue-500 hover:bg-gray-200" to="/hotel-accommodation-reservation">Hotel Bookings</nuxt-link>
            </li>
            <li>
              <nuxt-link class="block w-[230px] py-1 text-blue-500 hover:bg-gray-200" to="/management-information">Management Information</nuxt-link>
            </li>
            <li>
              <nuxt-link class="block w-[230px] py-1 text-blue-500 hover:bg-gray-200" to="/meet-and-great">Meet and Great</nuxt-link>
            </li>
            <li>
              <nuxt-link class="block w-[230px] py-1 text-blue-500 hover:bg-gray-200" to="/meeting-incentive-convention-and-exhibition">M.I.C.E</nuxt-link>
            </li>
            <li>
              <nuxt-link class="block w-[230px] py-1 text-blue-500 hover:bg-gray-200" to="/outbound-travel">Outbound Travel</nuxt-link>
            </li>
            <li>
              <nuxt-link class="block w-[230px] py-1 text-blue-500 hover:bg-gray-200" to="/travel-insurance">Travel Insurance</nuxt-link>
            </li>
          </ul>
        </div>
      </div>
      <div class="lg:mb-0 mb-4">
        <!-- Dropdown menu -->
        <div class="relative group">
          <span class="cursor-pointer">DESTINATIONS <i class="fa fa-angle-down"></i></span>
          <ul class="hidden absolute top-full left-0 bg-white border border-gray-300 p-4 group-hover:block">
            <li class="mb-1">
              <nuxt-link class="block px-2 py-1 text-blue-500 hover:bg-gray-200" to="/baku-trip">Baku</nuxt-link>
            </li>
            <li class="mb-1">
              <nuxt-link class="block px-2 py-1 text-blue-500 hover:bg-gray-200" to="/ganja-trip">Ganja</nuxt-link>
            </li>
            <li class="mb-1">
              <nuxt-link class="block px-2 py-1 text-blue-500 hover:bg-gray-200" to="/gabala-trip">Gabala</nuxt-link>
            </li>
            <li class="mb-1">
              <nuxt-link class="block px-2 py-1 text-blue-500 hover:bg-gray-200" to="/guba-trip">Guba</nuxt-link>
            </li>
            <li class="mb-1">
              <nuxt-link class="block px-2 py-1 text-blue-500 hover:bg-gray-200" to="/sheki-trip">Sheki</nuxt-link>
            </li>
            <li class="mb-1">
              <nuxt-link class="block px-2 py-1 text-blue-500 hover:bg-gray-200" to="/shusha-trip">Shusha</nuxt-link>
            </li>
            <li class="mb-1">
              <nuxt-link class="block px-2 py-1 text-blue-500 hover:bg-gray-200" to="/lankaran-trip">Lankaran</nuxt-link>
            </li>
            <li class="mb-1">
              <nuxt-link class="block px-2 py-1 text-blue-500 hover:bg-gray-200" to="/nakhchivan-trip">Nakhchivan</nuxt-link>
            </li>
          </ul>
        </div>
      </div>
      <div class="lg:mb-0 mb-4">
        <nuxt-link  class="txt-header hover:text-green-600 transition duration-200" to="/visa-processing-and-immigration-assistance">VISA SERVICES</nuxt-link>
      </div>
      <div class="lg:mb-0 mb-4">
        <nuxt-link class="txt-header hover:text-green-600 transition duration-200" to="/plan-your-trip">PLAN YOUR TRIP</nuxt-link>
      </div>
      <div class="lg:mb-0 mb-4">
        <nuxt-link class="txt-header hover:text-green-600 transition duration-200" to="/blog">BLOG</nuxt-link>
      </div>
      <div class="lg:mb-0 mb-4">
        <a class="txt-header hover:text-green-600 transition duration-200" href="">CONTACT US</a>
      </div>
    </div>
    <div class="text-center lg:mt-72">
      <h1 class="text-6xl font-medium	 text-white">Book your holiday</h1>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Navbar',
  methods: {
    getBackgroundStyle() {
      const isHomePage = this.$route.path === '/';
      return {
        height: isHomePage ? '100vh' : '75vh',
        backgroundImage: isHomePage
          ? 'url(' + require('~/assets/baku/baku-1.jpg') + ')'
          : 'url(' + require('~/assets/baku/baku-1.jpg') + ')',
      };
    },
  },

}
</script>
<style>

</style>
