<template>
    <div class="h-full">
        <div class="section1 section-padding rounded-b-lg">
            <div class="flex justify-between">
                <p class="text-white text-xl font-medium">Halo, <span class="font-thin">Nama!</span></p>
                <img style="width:44px;" src="~/assets/img/profpicplaceholder.png" alt="">
            </div>
            <p class="text-white text-3xl mt-3 pb-3 font-bold">Bagaimaa Kabarmu Hari ini?</p>
        </div>
        <div class="section2 section-padding">
            <div class="flex justify-between">
                <p class="font-bold text-xl">Apa yang ingin kamu <br> ceritakan hari ini?</p>
                <a class="self-end text-xs text-blue-500" href="#">Lihat Semua</a>
            </div>
            <div class="flex mt-5">
                <div class="card mr-3" style="background-color:#FE99B0;">
                    <p class="text-white text-xl p-4">Patah hati</p>
                </div>
                <div class="card" style="background-color:#229895;">
                    <p class="text-white text-xl p-4">Keluarga</p>
                </div>
            </div>
        </div>
        <div class="section3 section-padding">
           <h1 class="text-xl font-bold">Bagaimana <br> perasaanmu?</h1> 
           <div class="flex mt-5 justify-between">
                <div>
                    <div class="card-small">
                        <img src="~/assets/img/bahagia.png" alt="" srcset="">
                    </div>
                    <p class="text-sm text-center mt-0.5">Bahagia</p>
                </div>
                <div>
                    <div class="card-small">
                        <img class="" src="~/assets/img/kecewa.png" alt="" srcset="">
                    </div>
                    <p class="text-sm text-center mt-0.5">Kecewa</p>
                </div>
                <div>
                    <div class="card-small">
                        <img src="~/assets/img/marah.png" alt="" srcset="">
                    </div>
                    <p class="text-sm text-center mt-0.5">Marah</p>
                </div>
                <div>
                    <div class="card-small">
                        <img src="~/assets/img/sedih.png" alt="" srcset="">
                    </div>
                    <p class="text-sm text-center mt-0.5">Sedih</p>
                </div>  
           </div>
           <div class="w-full flex justify-center mt-4">
                <button class=" bg-button px-6 py-3 font-bold text-white rounded-full">Curhat Sekarang</button>
           </div>
           
        </div>
    </div>
</template>
<script>
export default {
    head(){
        return {
            title: "Home"
        }
    }
}
</script>
<style>
.section-padding{
    padding: 1.5rem;
}
.section1{
    background-image: linear-gradient(45deg,#64BCBE 75%,white);
}
.section3{
    padding-top: inherit;
}
.card{
    width: 269px;
    height: 123px;  
    @apply rounded-xl;
    box-shadow: 0 4px 8px 0 rgba(0,0,0,.12), 0 2px 4px 0 rgba(0,0,0,.08);
}
.card-small{
    width: 66px;
    height: 65px;
    background-color: #64BCBE;
    @apply rounded-xl flex items-center justify-center;     
}
.bg-button{
    background-color: #0E1B47;
}


</style>