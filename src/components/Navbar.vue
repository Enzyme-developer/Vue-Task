<template>
    <div class="w-full flex pt-[30px] justify-between flex-wrap">
        <div class="flex flex-col">
            <h1 class="font-medium text-3xl leading-[44px] text-[#101828]">Welcome, Jonathan</h1>
            <p class="text-sm font-normal text-[#475467] mt-1">View assessments and top scorers at a glance.</p>
        </div>
        <div>
            <Button />
        </div>
    </div>
</template>

<script>
    import Button from './Button.vue';

    export default {
    name: "Navbar",
    emits:['close'],
    components: { Button }
}
</script>