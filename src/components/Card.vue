<template>
    <div class="flex flex-col mt-8 overflow-scroll no-scrollbar ">
        <h1 class="font-semibold text-xl leading-8 mb-6">Recent workbooks</h1>

        <div class="overflow-x-scroll no-scrollbar flex flex-wrap md:flex-nowrap w-full space-x-0 space-y-4 md:space-y-0 md:space-x-8 ">
            
            <div class="flex flex-col p-4 w-full md:w-[330px] min-w-[330px] h-[268px] rounded-lg bg-[#ffffff] relative">
            <img @click="show = !show" src="../assets/hamburger.png" alt='toggle' class="flex self-end" />
            <div class="flex items-center">
                <img src='../assets/User-Research.png' alt='icon' class="w-[100px] h-[100px] mr-4" />
                <div>
                    <h1 class="text-[#101828] text-[16px] leading-6 font-semibold">UX Research</h1>
                    <p class="text-sm font-normal my-1 text-[#475467]">25 questions</p>
                    <p class="text-sm font-normal text-[#475467]">30 minutes</p>
                </div>
            </div>
            <p class="text-sm font-normal my-4 text-[#475467]">Used space Contains questions that will help improve your design thinking process to enhance your UX design.</p>
            <img src='../assets/cardImage1.png' class='mt-4' />
            <div v-if="show" class="shadow-xl bg-[#ffffff] w-[213px] p-[14px] flex flex-col rounded-lg absolute top-8 right-[11px]">
                <p class="cursor-pointer flex text-sm text-black font-normal p-[10px] rounded-lg bg-[#F9FAFB]"><img src='../assets/ShareNetwork.png' class="mr-2"/>Share workbook</p>
                <p class="cursor-pointer flex text-sm text-black font-normal p-[10px]"><img src='../assets/edit-02.png' class="mr-2"/>Edit</p>
                <p class="cursor-pointer flex text-sm text-black font-normal p-[10px]"><img src='../assets/Icon.png' class="mr-2"/>Delete</p>
            </div>
            <div v-else></div>
        </div>


        <div class="flex flex-col p-4 w-full md:w-[330px] min-w-[330px] h-[268px] rounded-lg bg-[#ffffff] relative">
            <img src="../assets/hamburger.png" alt='toggle' class="flex self-end" @click="show2 = !show2"/>
            <div class="flex items-center">
                <img src='../assets/UX-Principles.png' alt='icon' class="w-[100px] h-[100px] mr-4" />
                <div>
                    <h1 class="text-[#101828] text-[16px] leading-6 font-semibold">UX Research</h1>
                    <p class="text-sm font-normal my-1 text-[#475467]">25 questions</p>
                    <p class="text-sm font-normal text-[#475467]">30 minutes</p>
                </div>
            </div>
            <p class="text-sm font-normal my-4 text-[#475467]">Used space Contains questions that will help improve your design thinking process to enhance your UX design.</p>
            <img src='../assets/cardImage2.png' class='mt-4' />
             <div v-if="show2" class="shadow-xl bg-[#ffffff] w-[213px] p-[14px] flex flex-col rounded-lg absolute top-8 right-[11px]">
                <p class="cursor-pointer flex text-sm text-black font-normal p-[10px] rounded-lg bg-[#F9FAFB]"><img src='../assets/ShareNetwork.png' class="mr-2"/>Share workbook</p>
                <p class="cursor-pointer flex text-sm text-black font-normal p-[10px]"><img src='../assets/edit-02.png' class="mr-2"/>Edit</p>
                <p class="cursor-pointer flex text-sm text-black font-normal p-[10px]"><img src='../assets/Icon.png' class="mr-2"/>Delete</p>
            </div>
            <div v-else></div>
        </div>

        <div class="flex flex-col p-4 w-full md:w-[330px] min-w-[330px] h-[268px] rounded-lg bg-[#ffffff] relative">
            <img src="../assets/hamburger.png" alt='toggle' class="flex self-end" @click="show3 = !show3"/>
            <div class="flex items-center">
                <img src='../assets/Typography.png' alt='icon' class="w-[100px] h-[100px] mr-4" />
                <div>
                    <h1 class="text-[#101828] text-[16px] leading-6 font-semibold">UX Research</h1>
                    <p class="text-sm font-normal my-1 text-[#475467]">25 questions</p>
                    <p class="text-sm font-normal text-[#475467]">30 minutes</p>
                </div>
            </div>
            <p class="text-sm font-normal my-4 text-[#475467]">Used space Contains questions that will help improve your design thinking process to enhance your UX design.</p>
            <img src='../assets/cardImage3.png' class='mt-4' />
            <div v-if="show3" class="shadow-xl bg-[#ffffff] w-[213px] p-[14px] flex flex-col rounded-lg absolute top-8 right-[11px]">
                <p class="cursor-pointer flex text-sm text-black font-normal p-[10px] rounded-lg bg-[#F9FAFB]"><img src='../assets/ShareNetwork.png' class="mr-2"/>Share workbook</p>
                <p class="cursor-pointer flex text-sm text-black font-normal p-[10px]"><img src='../assets/edit-02.png' class="mr-2"/>Edit</p>
                <p class="cursor-pointer flex text-sm text-black font-normal p-[10px]"><img src='../assets/Icon.png' class="mr-2"/>Delete</p>
            </div>
            <div v-else></div>
        </div>

        
        <div class="flex items-center p-4 w-[116px] h-[268px] rounded-lg bg-[#ffffff]">
            <p class="flex items-center text-primary "><span class='text-2xl mb-1'>+</span> 2 more</p>
        </div>

    </div>
</div>
</template>

<script>
export default {
    name: 'Card',
    props: {
        icon: String,
        cardImage: String,
        questions: String,
        time: String,
        desc: String,
    },
    data() {
        return {
            show: false,
            show2: false,
            show3: false
        }
    }
}
</script>