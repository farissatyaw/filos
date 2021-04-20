<template>
    <div class="body-finished">
        <div class="card">
        <div class="">
            <svg class="flex ml-6" height="150" width="150">
                <circle cx="75" cy="75" r="60" stroke="black" stroke-width="0" fill="gray" />
            </svg>
            <h1 class="text-3xl font-bold mt-6">Waktu habis</h1>
        </div>
            
        <h2 class="text-center italic">Lanjut 30 menit?<br><NuxtLink to="/calling">Ya</NuxtLink>  / <NuxtLink to="/rate">Tidak</NuxtLink></h2>
    </div>
    </div>
</template>
<script>
export default {
    head(){
        return {
            title: "Continue?"
        }
    }
}
</script>
<style>
.body-finished{
    background-image: url(~/assets/img/image14.png);
    background-size: cover;
    @apply flex items-center justify-center py-10;
}
.card{
    background-color: rgba(255, 255, 255, 0.7);
    height: 649px;
    width: 317px;
    @apply rounded-xl flex flex-col justify-around items-center p-6;
}
</style>