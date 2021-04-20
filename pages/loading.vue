<template>
    <div class="body-loading">
        <div class="card-loading">
        <div class="">
            <svg class="flex ml-6" height="150" width="150">
                <circle cx="75" cy="75" r="60" stroke="black" stroke-width="0" fill="gray" />
            </svg>
            <h1 class="text-3xl font-bold mt-6">Menunggu . . .</h1>
        </div>
            
        <h2 class="text-center italic text-sm">When education is not liberating, the dream of the oppressed is to become the oppressor.</h2>
    </div>
    </div>
</template>
<script>

export default {
    head(){
        return {
            title: "Searching for partner"
        }
    },
    mounted(){
        setTimeout(function(){
            window.location.href="/calling"
        }, 5000)}
}
</script>
<style>
.body-loading{
    background-image: url(~/assets/img/image14.png);
    background-size:cover; 
    @apply flex items-center justify-center py-10;
}
.card-loading{
    background-color: rgba(255, 255, 255, 0.7);
    height: 649px;
    width: 317px;
    @apply rounded-xl flex flex-col justify-around items-center p-6;
}
</style>