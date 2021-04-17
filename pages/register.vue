<template>
    <div class="h-screen p-4 bg-red flex flex-col">
        <div class="mt-3">
            <div class="">
                <h1 class="text-3xl font-bold ml-4">Sudah <br>Punya <br>Akun?</h1>
            </div>
            <div class="">
                <div class="card p-4 my-6 flex flex-col">
                    <p>Nama : </p>
                    <input class="input-line" type="text" name="password" >
                    <p>Password : </p>
                    <input class="input-line" type="text" name="password" >
                    <button class="bg-blue px-4 py-1 rounded-lg mt-3"><span class="text-white">Login</span></button>
                </div>
                
                <p class="text-sm text-center">Belum Memiliki Akun? <span class="font-bold">Daftar Sekarang</span> </p>
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
.input-line{  
    border-bottom: 1px solid #858586;
    @apply mb-3
}
.bg-red{
    background-color: #65BCBF;
}
.bg-blue{
    background-color: #0D1B46;
}
.card{
    @apply bg-white rounded-lg shadow-2xl
    
}
</style>