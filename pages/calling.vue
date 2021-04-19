<template>
    <div class="card">
        <div class="">
            <svg class="flex ml-10" height="150" width="150">
                <circle cx="75" cy="75" r="60" stroke="black" stroke-width="0" fill="gray" />
            </svg>
            <h1 class="text-3xl font-bold mt-6">Edward Newgate</h1>
            <h2 id="safetimer" class="text-center text-2xl">30:00</h2>
        </div>
        <div class="flex">
            
            <NuxtLink to="/finished"><img src="~/assets/img/end-call.png" style="width:50px;" alt=""></NuxtLink>
            
        </div>  
        
    </div>
</template>
<script>
export default {
    head(){
        return {
            title: "Calling Edward Newgate"
        }
    },
    mounted(){
        var sec = 1800;
        var minute = 0;
        var tempsec= 0;
        var timer = setInterval(function(){
            minute = Math.floor(sec/60);
            tempsec = sec%60;
            document.getElementById('safetimer').innerHTML=minute+':'+tempsec;
            sec--;
            if(sec<0){
                clearInterval(timer);
                window.location.href="/finished"
            }
        }, 1000);
    }
}
</script>
<style>
body{
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