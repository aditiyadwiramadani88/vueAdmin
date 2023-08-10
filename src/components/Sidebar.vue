<script>
// import { Chart } from 'chart.js';
import Chart from './Chart.vue';



export default {
    data() {
        return {};
    },
    components: { Chart }
}
</script>

<template> 
<div class="flex justify-start bg-slate-50 ">   
        <!-- sidebar -->
        <div class="md:text-2xl text-lg min-h-screen bg-pink-50  rounded-md w-52 shadow-lg">
            <!-- title -->
            <div class="mt-4">
                <h1 class="font-bold text-center text-gray-600">Admin</h1>
            </div>
            <!-- end title -->

            <!-- main menu -->
            <div class="my-8 ml-4">
                <p class="uppercase text-gray-300 text-[10px]">Main Menu</p>
                <div class="my-2 flex  text-gray-600 cursor-pointer hover:text-orange-400">
                    <i class="fa-solid mt-2 fa-house text-[16px]"></i>
                    <p class="ml-2 text-[16px]">Home</p>    
                </div>

                <div class="my-4 flex  text-gray-600 cursor-pointer hover:text-orange-400">
                    <i class="fa-solid mt-2 fa-shop  text-[16px]"></i>
                    <p class="ml-2 text-[16px]">Product</p>    
                </div>
    
                <div class="my-4 flex  text-gray-600 cursor-pointer hover:text-orange-400">
                    <i class="fa-solid mt-2 fa-chart-simple  text-[16px]"></i>
                    <p class="ml-2 text-[16px]">Analitycs</p>    
                </div>

                <div class="my-4 flex  text-gray-600 cursor-pointer hover:text-orange-400">
                    <i class="fa-solid mt-2 fa-user-group  text-[16px]"></i>
                    <p class="ml-2 text-[16px]">Users</p>    
                </div>
            </div>
            <!-- end mainmenu -->

            <!-- main menu -->
            <div class="my-8 ml-4">
                <p class="uppercase text-gray-300 text-[10px]">User Menu</p>
                <div class="my-2 flex  text-gray-600 cursor-pointer hover:text-orange-400">
                    <i class="fa-solid mt-2 fa-user text-[16px]"></i>
                    <p class="ml-2 text-[16px]">Profile</p>    
                </div>

                <div class="my-4 flex  text-gray-600 cursor-pointer hover:text-orange-400">
                    <i class="fa-solid mt-2 fa-gear  text-[16px]"></i>
                    <p class="ml-2 text-[16px]">Setting</p>    
                </div>
    
                <div class="my-4 flex  text-gray-600 cursor-pointer hover:text-orange-400">
                    <i class="fa-solid fa-arrow-right-from-bracket mt-2  text-[16px]"></i>
                    <p class="ml-2 text-[16px]">Logout</p>    
                </div>

               
            </div>
            <!-- end mainmenu -->
        </div>
        <!-- endsidebar -->
        <!-- content -->
        <div class="col-start-2 col-span-4 mx-auto ">

            <div class="grid grid-cols-4 gap-4  mt-16">
                <div class=" bg-white text-gray-600  text-sm py-4 px-8 rounded-lg shadow-lg">
                    <div class="flex">
                        <div class="bg-blue-400 w-10 text-center rounded-lg mr-4">
                            <i class="fa-solid mt-3 fa-cart-shopping text-white  text-[16px]"></i>
                        </div>
                        <div>
                            <p>Penjualan</p>
                            <p class="font-bold">Rp.40000.000</p>
                        </div>
                    </div>
                </div>
                <div class=" bg-white text-gray-600  text-sm py-4 px-8 rounded-lg shadow-lg">
                    <div class="flex">
                        <div class="bg-orange-400 w-10 text-center rounded-lg mr-4">
                            <i class="fa-solid mt-3 fa-eye text-white  text-[16px]"></i>
                        </div>
                        <div>
                            <p>Statistik</p>
                            <p class="font-bold">40 Views</p>
                        </div>
                    </div>
                </div>
                <div class=" bg-white text-gray-600  text-sm py-4 px-8 rounded-lg shadow-lg">
                    <div class="flex">
                        <div class="bg-pink-400 w-10 text-center rounded-lg mr-4">
                            <i class="fa-solid mt-3 fa-shop text-white  text-[16px]"></i>
                        </div>
                        <div>
                            <p>Product</p>
                            <p class="font-bold">50 Product</p>
                        </div>
                    </div>
                </div>
                <div class=" bg-white text-gray-600  text-sm py-4 px-8 rounded-lg shadow-lg">
                    <div class="flex">
                        <div class="bg-purple-400 w-10 text-center rounded-lg mr-4">
                            <i class="fa-solid mt-3 fa-shop text-white  text-[16px]"></i>
                        </div>
                        <div>
                            <p>Pembelian</p>
                            <p class="font-bold">Rp. 30000.000</p>
                        </div>
                    </div>
                </div>
                
            </div>


            <div class="rounded-lg mx-auto py-4 px-4 my-8 shadow-lg bg-white ">
                <h1 class="font-bold text-lg">Statictic Buy</h1>
                <Chart />

            </div>


        </div>
        <!-- end content -->
</div>

</template>