<template>
    <div class="h-full bg-blue">
        <div class="mb-2">
            <div class="half flex items-center justify-center">
                <img class="" src="~/assets/img/gambar1.png" alt="">
            </div>
            <div class="half text-center rounded-tl-lg bg-white-opacity">
                <div class="p-8 mb-4 flex flex-col justify-between">
                    <h1 class="text-4xl font-bold text-heading mb-3">Selamat Datang di Filos</h1>
                    <p class="m-5 text-xl text-center">Halo, Bagaimana Harimu?<br>Apakah baik-baik saja?<br>Atau malah tidak?</p> 
                    <div class="flex justify-end">
                        <a href="/login">
                            <!-- <svg xmlns="http://www.w3.org/2000/svg" class="h-12 w-12" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17 8l4 4m0 0l-4 4m4-4H3" />
                            </svg> -->
                            <img src="~/assets/img/arrow.png" alt="">
                        </a>  
                    </div>
                                    
                </div>
            </div>     
        </div>
          
    </div>
</template>
<script>
export default {
    head(){
        return {
            title: "About the app"
        }
    }
}
</script>
<style>
.half{
    height: 50vh;
}
.bg-blue{
    background-image: url(~/assets/img/image14.png);
}
.bg-white-opacity{
    background-color: rgba(255,255,255,0.7);
}
.text-heading{
    color:#0E1B47;
}
body{
    max-height: 731px;
    max-width: 411px;
}
</style>