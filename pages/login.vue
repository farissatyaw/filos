<template>
    <div class="h-screen p-4 bg-turqoise flex flex-col">
        <div class="mt-8">
            <div class="mb-3">
                <h1 class="text-4xl font-bold ml-4">Sudah <br>Punya <br>Akun?</h1>
            </div>
            <div class="mt-3">
                <div class="card p-4 my-6 flex flex-col">
                    <p class="text-lg mb-4">Username : </p>
                    <input class="input-line mb-6" type="text" name="username" >
                    <p class="text-lg mb-4">Password : </p>
                    <input class="input-line mb-3" type="password" name="password" >
                    <div class="flex justify-center mt-6 mb-3">
                        <a href="/home" class="bg-blue rounded-full text-white py-2 px-10">Login</a>
                    </div>   
                </div>     
                <p class="text-sm text-center">Belum Memiliki Akun? <a href="/register" class="font-bold">Daftar Sekarang</a> </p>
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
}
.bg-turqoise{
    background-image: url(~/assets/img/image14.png);
    background-size: cover;
}
.bg-blue{
    background-color: #0D1B46;
}
.card{
    background-color: rgba(255,255,255,0.7);
    @apply rounded-xl shadow-2xl;
    
}
input{
    background: none;
}
</style>