<template>
    <div>
        <div class="flex flex-col mt-4 md:mt-0 ">
            <button  @click="show = !show" :style="{ color: 'white'}" class=" rounded-md text-sm font-medium text-white leading-[22px] text-white flex border-0 outline-0 w-[191px] h-[42px] bg-primary items-center justify-center">
                <p class="text-sm font-medium leading-[22px] mr-2">create assessment</p>
                <img src='../assets/chevron-down.png' />
            </button>
            <div v-if="show" class="w-[191px] flex flex-col rounded-md mt-2 bg-[#fff] shadow-xl">
                <p class="text-sm text-black font-normal p-[10px] bg-[#F9FAFB]">New assessment</p>
                <p class="text-sm text-black font-normal p-[10px]">SimplifiedUx workbook</p>
            </div>
            <div v-else class="w-[191px] flex flex-col rounded-md mt-2 bg-[#fff] shadow-xl"></div>
        </div>
    </div>
</template>

<script>

export default {
    name: 'Button',
    props: {
        buttonText: String,
        dropdown: String,
        optionA: String,
        optionB: String
    },
    data() {
        return {
            show: true
        }
    }
}
</script>