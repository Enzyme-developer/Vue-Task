<template>
    <div>
        <h1 class="mt-6 mb-10 font-medium text-xl leading-8">Recent results</h1>

        <div class="bg-[#fff] px-6 py-[21px] rounded-lg">
            <h1 class="font-medium text-xl leading-8">Top 3 scorers</h1>
            <p class="text-sm leading-[22px] font-normal">See the top scorers within each workbook</p>
        </div>

        <div class="flex justify-between items-center px-6 h-10 h-7 bg-[#EAECF0]">
            <h1 class="font-medium text-lg">UX Research</h1>
            <img src="../assets/collapse.png" @click="table1 = !table1"/>
        </div>
        <table v-if="table1" class="text-sm w-full table border-spacing-24 text-left pl-6">
            <thead class="px-6">
                <tr class="h-12">
                <th>Name</th>
                <th>Email</th>
                <th class="flex items-center mt-[15px]">Role<span><img class='ml-1' src='../assets/help-circle.png' /></span></th>
                <th>Score</th>
                <th>Time used</th>
                <th></th>
                </tr>
            </thead>
            <tbody>
                <tr class="h-12 border border-[#e3e3e3] bg-[#fff]">
                <td>Olivia Rhye</td>
                <td>olivia@untitledui.com</td>
                <td>Product designer</td>
                <td>95%</td>
                <td>7:29</td>
                <td><img src="../assets/collapse.png" class="rotate-90" alt='expand' /></td>
                </tr>
                <tr class="h-12 border border-[#e3e3e3] bg-[#fff]">
                <td>Phoenix Baker</td>
                <td>phoenix@untitledui.com</td>
                <td>Product manager</td>
                <td>82%</td>
                <td>19:30</td>
                <td><img src="../assets/collapse.png" class="rotate-90" alt='expand' /></td>
                </tr>
                <tr class="h-12 border border-[#e3e3e3] bg-[#fff]">
                <td>Lana Steiner</td>
                <td>lana@untitledui.com</td>
                <td>Frontend developer</td>
                <td>75%</td>
                <td>21:45</td>
                <td><img src="../assets/collapse.png" class="rotate-90" alt='expand' /></td>
                </tr>
            </tbody>
            </table>
            <table v-else></table>


            <div class="flex justify-between items-center px-6 h-10 h-7 bg-[#EAECF0]">
                <h1 class="font-medium text-lg">UX Principles</h1>
                <img src="../assets/collapse.png" @click="table2 = !table2" />
            </div>
            <table  v-if="table2" class="text-sm w-full table border-spacing-24 text-left pl-6">
            <thead class="px-6">
                <tr class="h-12">
                <th>Name</th>
                <th>Email</th>
                <th class="flex items-center mt-[15px]">Role<span><img class='ml-1' src='../assets/help-circle.png' /></span></th>
                <th>Score</th>
                <th>Time used</th>
                <th></th>
                </tr>
            </thead>
            <tbody>
                <tr class="h-12 border border-[#e3e3e3] bg-[#fff]">
                <td>Olivia Rhye</td>
                <td>olivia@untitledui.com</td>
                <td>Product designer</td>
                <td>95%</td>
                <td>7:29</td>
                <td><img src="../assets/collapse.png" class="rotate-90" alt='expand' /></td>
                </tr>
                <tr class="h-12 border border-[#e3e3e3] bg-[#fff]">
                <td>Phoenix Baker</td>
                <td>phoenix@untitledui.com</td>
                <td>Product manager</td>
                <td>82%</td>
                <td>19:30</td>
                <td><img src="../assets/collapse.png" class="rotate-90" alt='expand' /></td>
                </tr>
                <tr class="h-12 border border-[#e3e3e3] bg-[#fff]">
                <td>Lana Steiner</td>
                <td>lana@untitledui.com</td>
                <td>Frontend developer</td>
                <td>75%</td>
                <td>21:45</td>
                <td><img src="../assets/collapse.png" class="rotate-90" alt='expand' /></td>
                </tr>
            </tbody>
            </table>
            <table v-else></table>



            <div class="flex justify-between items-center px-6 h-10 h-7 bg-[#EAECF0]">
                <h1 class="font-medium text-lg">Typography</h1>
                <img src="../assets/collapse.png" @click="table3 = !table3"/>
            </div>
            <table  v-if="table3" class="text-sm w-full table border-spacing-24 text-left px-6 no-scrollbar">
            <thead class="px-6">
                <tr class="h-12 font-normal">
                <th>Name</th>
                <th>Email</th>
                <th class="flex items-center mt-[15px]">Role<span><img class='ml-1' src='../assets/help-circle.png' /></span></th>
                <th>Score</th>
                <th>Time used</th>
                <th></th>
                </tr>
            </thead>
            <tbody>
                <tr class="h-12 border border-[#e3e3e3] bg-[#fff]">
                <td>Olivia Rhye</td>
                <td>olivia@untitledui.com</td>
                <td>Product designer</td>
                <td>95%</td>
                <td>7:29</td>
                <td><img src="../assets/collapse.png" class="rotate-90" alt='expand' /></td>
                </tr>
                <tr class="h-12 border border-[#e3e3e3] bg-[#fff]">
                <td>Phoenix Baker</td>
                <td>phoenix@untitledui.com</td>
                <td>Product manager</td>
                <td>82%</td>
                <td>19:30</td>
                <td><img src="../assets/collapse.png" class="rotate-90" alt='expand' /></td>
                </tr>
                <tr class="h-12 border border-[#e3e3e3] bg-[#fff]">
                <td>Lana Steiner</td>
                <td>lana@untitledui.com</td>
                <td>Frontend developer</td>
                <td>75%</td>
                <td>21:45</td>
                <td><img src="../assets/collapse.png" class="rotate-90" alt='expand' /></td>
                </tr>
            </tbody>
            </table>
            <table v-else></table>
    </div>
</template>

<script>

    export default {
    name: 'Table',
    // props: {
    //     buttonText: String,
    //     dropdown: String,
    //     optionA: String,
    //     optionB: String
    //     }
    data() {
        return {
            table1: true,
            table2: true,
            table3: true
        }
    }
    }
</script>