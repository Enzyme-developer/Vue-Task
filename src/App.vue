<script>
import Card from './components/Card.vue'
import Navbar from './components/Navbar.vue'
import Upgrade from './components/Upgrade.vue';
import User from './components/User.vue';
import Table from './components/Table.vue';

export default {
  name: 'App',
  components: {
    Card,
    Navbar,
    Upgrade,
    User,
    Table
},
data() {
        return {
            nav: false
        }
    }
}
</script>

<template>
  <div class="flex overflow-scroll relative no-scrollbar">
    <img src='./assets/hamburger.png'  @click="nav = !nav" class='absolute md:hidden right-4 top-4 '/>
    <!-- sidebar -->
    <div v-if="nav" class="absolute md:hidden md:relative z-20 bg-[#fff] flex-col h-[100vh] min-w-[290px]  w-[290px] max-h-[100vh] overflow-auto no-scrollbar">
      <div class="px-7 mt-[40px]">
        <div class="flex mb-3 items-center">
          <img src="./assets/bar-chart-square-02.png" class="mr-3" alt='icon'/>
          <p class="font-semibold text-base leading-6 text-primary">Dashboard</p>
        </div>
        <div class="flex mb-[40px] items-center">
          <img src="./assets/user.png" class="mr-3" alt='icon'/>
          <p class="font-semibold text-base leading-6">Team</p>
        </div>

        <div class="flex mb-3 items-center">
          <img src="./assets/support.png" class="mr-3" alt='icon'/>
          <p class="font-semibold text-base leading-6">Support</p>
        </div>
        <div class="flex items-center">
          <img src="./assets/settings-01.png" class="mr-3" alt='icon'/>
          <p class="font-semibold text-base leading-6">Settings</p>
        </div>

      </div>

      <div class="w-full flex px-4">
        <Upgrade />
      </div>
      <div class="w-full flex px-4">
        <User />
      </div>
    </div>
    <div v-else></div>

    <div class="hidden md:flex md:relative z-20 bg-[#fff] flex-col h-[100vh]  w-[290px] max-h-[100vh] overflow-auto no-scrollbar">
      <div class="px-7 mt-[40px]">
        <div class="flex mb-3 items-center">
          <img src="./assets/bar-chart-square-02.png" class="mr-3" alt='icon'/>
          <p class="font-semibold text-base leading-6 text-primary">Dashboard</p>
        </div>
        <div class="flex mb-[40px] items-center">
          <img src="./assets/user.png" class="mr-3" alt='icon'/>
          <p class="font-semibold text-base leading-6">Team</p>
        </div>

        <div class="flex mb-3 items-center">
          <img src="./assets/support.png" class="mr-3" alt='icon'/>
          <p class="font-semibold text-base leading-6">Support</p>
        </div>
        <div class="flex items-center">
          <img src="./assets/settings-01.png" class="mr-3" alt='icon'/>
          <p class="font-semibold text-base leading-6">Settings</p>
        </div>

      </div>

      <div class="w-full flex px-4">
        <Upgrade />
      </div>
      <div class="w-full flex px-4">
        <User />
      </div>
    </div>

    <!-- main -->
    <div class="w-full bg-[#F9FAFB] h-[100vh] px-6 overflow-auto no-scrollbar">
      <Navbar />
      <Card />
      <Table />
    </div>
  </div>
</template>