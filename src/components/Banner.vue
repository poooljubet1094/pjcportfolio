<template>
    <div class="grid place-items-center text-center p-5">
        <div class="text-4xl font-extrabold tracking-wider flex justify-center">Frontend, Backend & Mobile Developer</div>
        <div class="text-2xl tracking-wider flex justify-center mt-6">I design software from scratch using SOLID principles.</div>
        <div class="w-full flex justify-center">
            <img :src="avatar" class="h-72 w-72"/>
        </div>
    </div>
</template>

<script>
import avatar from '../assets/avatar.png'

export default {
    name: 'BannerComponent',
    data: function () {
        return {
            avatar: avatar
        }
    },
}
</script>